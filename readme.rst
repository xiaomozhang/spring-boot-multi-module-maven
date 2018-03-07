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


Then go to; localhost:8080

This project has 2 spring boot projects; api, web.
When web project runs it creates itself and it also creates api project. So, both modules run in single tomcat server.
Additionally, api module can run by itself since it's not dependent to web module.


