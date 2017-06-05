# Centos 编译安装 PHP 5.6


#### 安装常规工具

```
yum install -y gcc gcc-c++ libxml2-devel openssl-devel libcurl-devel libjpeg-devel libpng-devel libicu-devel openldap-devel 

```


#### 下载php 5.6 [tar包 ](http://php.net/downloads.php)

```
tar -zxvf php-5.6.15.tar

cd php-5.6.15

 ./configure --prefix=/usr/local/php --with-config-file-path=/usr/local/php/etc --enable-fpm --with-fpm-user=php-fpm --with-fpm-group=www --enable-mysqlnd --with-mysql=mysqlnd --with-mysqli=mysqlnd --with-pdo-mysql=mysqlnd --enable-opcache --enable-mbstring --enable-soap --enable-zip --enable-bcmath --with-openssl --with-zlib --with-curl --with-gd --with-zlib-dir=/usr/lib --with-png-dir=/usr/lib --with-jpeg-dir=/usr/lib --with-mhash 


make && make install 

 ```

 #### 参考文档

 1. [PHP 5.6.15 编译安装](http://dengxi.blog.51cto.com/4804263/1710479)
 2. [CentOS下PHP 5.6编译安装](https://my.oschina.net/u/150705/blog/473836)
 3. [centos6.5安装php开发环境](https://www.zybuluo.com/phper/note/79313)