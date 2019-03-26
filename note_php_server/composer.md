# "https://docs.phpcomposer.com/00-intro.html#Installation-\*nix"


#包管理工具
* 管理package 和library
* 做为全局到依赖使用

#依赖管理工具
* 管理package 和library

#安装Composer

* 安装composer到项目目录
1. curl -s  (composer web site)/installer|php  检查php配置，下载phar归档文件，里面可以包含任何文件，并且可以在php命令下执行
2. curl -s  (composer web site)installer|php -- --install-dir=bin

这两个步骤到作用是？

#example
在项目下composer.json下添加日志组件
{ "require": { "monolog/monolog": "1.2.\*" }}

# packagelist
https://www.jianshu.com/p/adcae6213e9b
