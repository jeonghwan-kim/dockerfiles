jeonghwan/mysql:5.6
====================

Mysql on ubuntu 14.04

Build:

```
$ docker build --tag jeonghwan/msyql:5.6 .
```

Usage:

```
$ docker run --name mysql -it jeonghwan/mysql:5.6
$ server mysql status
$ server mysql start
$ mysql
```
