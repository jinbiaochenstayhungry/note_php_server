#mac 下配置php.ini

1. mac下的php版本综述
mac下自带php 版本 使用whereis php可以查看php 版本
默认在/usr/bin/php


使用brew安装php版本，方便后续extension安装

brew install php@7.1

使用cakebrew 解决安装php的权限问题


修改默认版本
xport PATH="/usr/local/Cellar/php71/7.1.8_20/bin:$PATH"


Installing dependencies for php@7.1: apr, openssl, apr-util, aspell, autoconf, brotli, c-ares, libidn, libmetalink, libssh2, jansson, jemalloc, libev, libevent, nghttp2, openldap, rtmpdump, curl-openssl, libtool, unixodbc, freetds, libpng, freetype, pcre, pkg-config, gdbm, readline, sqlite, xz, python, glib, gmp, icu4c, jpeg, libpq, libzip, mhash, mcrypt, tidy-html5 and webp






2. 了解extension安装

php的extension是一下c语言模块，可以单独安装到lib目录中？





3. php.ini

* 在mac下没有这个文件，只有php.ini.default ,也就是这个配置文件不是必须的。

查看方法
https://blog.csdn.net/anycodes/article/details/
php -i  


* .修改https://blog.csdn.net/yxys01/article/details/78036834




4. 安装额外扩展

* 安装 magento后遇到ext缺失，如何安装
magento/product-community-edition 2.3.0 requires ext-intl * -> the requested PHP extension intl is missing from your system.

 To enable extensions, verify that they are enabled in your .ini files:
   - /etc/php.ini
