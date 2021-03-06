# swoole-vmstat

## 演示地址
* http://vmstat.val.xyz/

## 依赖

* PHP 5.3+
* Swoole 1.7.16
* Linux, OS X and basic Windows support (Thanks to cygwin)

## 安装 Swoole扩展

1. Install via pecl
    
    ```
    pecl install swoole
    ```

2. Install from source

    ```
    sudo apt-get install php5-dev
    git clone https://github.com/swoole/swoole-src.git
    cd swoole-src
    phpize
    ./configure
    make && make install
    ```
    
## 运行

	1. cd swoole-vmstat/server
	2. php server.php
	3. 修改web目录下stats.js代码 var ws = new ReconnectingWebSocket("ws://192.168.1.10:8888"); 改成服务器的IP
	4. 用浏览器打开web目录下的index.html

## 运行结果

1. 打开页面如下所示
![one](https://raw.githubusercontent.com/smalleyes/swoole-vmstat/master/doc/vmstat-web.png)
![two](https://raw.githubusercontent.com/smalleyes/swoole-vmstat/master/doc/vmstat-web1.png)

## nginx配置文件

	1. 在doc/swoole-vmstat.conf
## workerman实现
	1.github地址 https://github.com/walkor/workerman-vmstat
