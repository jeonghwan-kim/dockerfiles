jeonghwan/node:4.2.3
====================

Node, Npm, Forever on ubuntu 14.04

Build:

```
$ docker build --tag jeonghwan/node:4.2.3 .
```

Usage:

```
$ docker run --name node -it jeonghwan/node:4.2.3
$ node --version
v4.2.3
$ npm --version
v2.14.7
forever --version
v0.15.1
```
