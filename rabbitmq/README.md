
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
remote: Enumerating objects: 6199, done.
remote: Total 6199 (delta 0), reused 0 (delta 0), pack-reused 6199
Receiving objects: 100% (6199/6199), 2.62 MiB | 274 KiB/s, done.
Resolving deltas: 100% (4306/4306), done.
[root@zhangyz ~]# cd rabbitmq-c && mkdir build && cd build
[root@zhangyz build]# /usr/local/cmake/bin/cmake --version
cmake version 2.8.12.2
[root@zhangyz build]# 
[root@zhangyz build]# /usr/local/cmake/bin/cmake ..
-- The C compiler identification is GNU 4.4.7
-- Check for working C compiler: /usr/bin/cc
-- Check for working C compiler: /usr/bin/cc -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- CMAKE_BUILD_TYPE not specified. Creating Release build
-- Found C inline keyword: inline
-- Looking for getaddrinfo
-- Looking for getaddrinfo - found
-- Looking for socket
-- Looking for socket - found
-- Looking for poll
-- Looking for poll - found
-- Looking for clock_gettime in rt
-- Looking for clock_gettime in rt - found
-- Looking for posix_spawnp in rt
-- Looking for posix_spawnp in rt - found
-- Found OpenSSL: /usr/lib64/libssl.so;/usr/lib64/libcrypto.so (found suitable version "1.0.1e", minimum required is "0.9.8") 
-- Looking for include file pthread.h
-- Looking for include file pthread.h - found
-- Looking for pthread_create
-- Looking for pthread_create - not found
-- Looking for pthread_create in pthreads
-- Looking for pthread_create in pthreads - not found
-- Looking for pthread_create in pthread
-- Looking for pthread_create in pthread - found
-- Found Threads: TRUE  
-- Performing Test HAVE_GNU90
-- Performing Test HAVE_GNU90 - Failed
-- Performing Test HAVE_C90
-- Performing Test HAVE_C90 - Failed
-- Found POPT: /usr/include  
-- Could NOT find XMLTO (missing:  XMLTO_EXECUTABLE) 
-- Found Doxygen: /usr/bin/doxygen (found version "1.6.1") 
-- Building rabbitmq as a shared library - yes
-- Building rabbitmq as a static library - yes
-- Configuring done
-- Generating done
-- Build files have been written to: /usr/local/src/rabbitmq-c/build
[root@zhangyz build]# 

```
