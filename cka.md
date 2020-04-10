23.
24.创建一个持久卷，名称为app-config，容量为1Gi，访问模式为ReadWriteOnce 卷的类型是hostPath，它的位置是/srv/app-confi

`apiVersion: v1
kind: PersistentVolume
metadata:
  name: app-config
spec:
  capacity:
    storage: 1Gi
  accessModes:
    - ReadWriteOnce
  hostPath:
    path: /srv/app-config `
    