.. image:: https://travis-ci.org/xiaomozhang/spring-boot-multi-module-maven.svg?branch=master
   :target: https://travis-ci.org/xiaomozhang/spring-boot-multi-module-maven

spring-boot-multi-module-maven
~~~~~~~~~~~~

这个是一个多模块maven项目. 模块包含了api和web.

使用spring boot方式运行:

(1)清除并编译当前文件夹
  webDemoProject>mvn clean install
(2)idea配置sringboot编译启动

.. image:: image/springbootRunConfig.jpg

然后启动完成没有报错;在浏览器中输入 localhost:8080
~~~~~~~~~~~~~~
踩过的坑或注意事项
~~~~~~~~~~~~~~
1、spring boot打包插件兼容性
   spring-boot-maven-plugin 1.5.10版本的打包控件打出来的jar包是无法访问jsp的，直接404，即使你的jsp文件打包进去了。
   spring-boot-maven-plugin 1.4.2版本就是可以的，我不知道这两个版本打包控件有什么区别，有知道的大神可以讲讲。




