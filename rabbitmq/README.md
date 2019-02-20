
### 安装 boost-1.47.0

https://www.boost.org/users/history

下载相关文件 

```shell
[root@zhangyz ~]# wget https://jaist.dl.sourceforge.net/project/boost/boost/1.47.0/boost_1_47_0.tar.gz
[root@zhangyz ~]# tar -xf boost_1_47_0.tar.gz -C /usr/local/src
[root@zhangyz ~]# cd /usr/local/src
[root@zhangyz src]# ./bootstrap.sh
[root@zhangyz src]# ./bjam
......
```

运行大概5分钟到10分钟的样子会结束

### 安装 rabbitmq-c

https://github.com/alanxz/rabbitmq-c

下载相关文件

```shell
[root@zhangyz ~]# git clone https://github.com/alanxz/rabbitmq-c
[root@zhangyz ~]# cd rabbitmq-c && mkdir build && cd build
[root@zhangyz build]# /usr/local/cmake/bin/cmake --version
cmake version 2.8.12.2
[root@zhangyz build]# 
[root@zhangyz build]# /usr/local/cmake/bin/cmake ..
[root@zhangyz build]# cmake --build .
[root@zhangyz build]# make 
[root@zhangyz build]# make install 
```
