#  **FCat** 
FCat是基于Angular+SpringCloud的企业级基础功能框架(户权限管理、区域管理、GIS地图、......)，其核心设计目标是分离前后端、开发快速、学习简单、功能强大、不重复造轮子，其目标是帮助企业搭建一套基础功能框架；
核心技术：angualr、Spring Cloud、OAuth2、jwt、Spring Cloud Security、Eureka、Zuul、Hystrix、Feign、Ribbon、Redis、Mybatis、Mysql。

 **QQ群号（1群）：549141844**   

[^_^] 演示地址： http://fcat.xfdmao.com    

[【FCat-基于session共享分支】](https://gitee.com/xfdm/FCat)   
[【FCat-基于Oauth2、jwt鉴权分支】](https://gitee.com/xfdm_admin/Angular-SpringCloud-Oauth2)

【CSDN教程地址】：http://edu.csdn.net/course/detail/6358
# 架构设计 
![img](http://on-img.com/chart_image/5a20b3f5e4b0add9c9f9ed64.png)

## 前端技术：Angular；
## 后端技术：SpringCloud；
- Eureka  
    服务器用作服务注册服务器。
    一个java客户端，用来简化与服务器的交互、作为轮询负载均衡器，并提供服务的故障切换支持。
- Zuul  
    基于JVM路由和服务端的负载均衡器
    类似nginx，反向代理的功能
- Hystrix  
    提供了熔断、隔离、Fallback、cache、监控等功能，能够在一个、或多个依赖同时出现问题时保证系统依然可用。
- Feign  
    是声明式、模板化的http客户端。旨在用最少的开销和代码将您的代码连接到http apis。
- Ribbon  
    提供客户端的软件负载均衡算法
- Redis  
    存储热点数据
- OAuth2  
    一种授权框架，提供了一套详细的授权机制（指导）。用户或应用可以通过公开的或私有的设置，授权第三方应用访问特定资源。
- JWT
    提供了一种用于发布接入令牌（Access Token),并对发布的签名接入令牌进行验证的方法。 令牌（Token）本身包含了一系列声明，应用程序可以根据这些声明限制用户对资源的访问。
- Security  
    提供声明式的安全访问控制解决方案的安全框架

## 开发环境
- node-v6.11.0-x64.msi
- redis3.X
- jdk1.8
- MySQL Server 5.6
- maven3.X
- IntelliJ IDEA 
- webstorm


## 部署项目
#### 前端   
```
npm config set registry https://registry.npm.taobao.org
npm install -g @angular/cli
cd fcat-angular
npm install
npm start
```
#### 后台
```
后台依次启动：CenterBootstrap、ConfigBootstrap、AuthApplication、GateBootstrap、UserBootstrap  
```
#### 访问
```
http://localhost:4200 
```

## 功能    
- 项目搭建、架构设计  
- 用户管理     
- 菜单管理  
- 组织类型管理  
- 组织架构管理————组织管理、关联用户、组织授权  
  
 
## 前端效果
## 前端效果
![img](http://image.xfdmao.com/fcat/demo/fcat-login.png)
![img](http://image.xfdmao.com/fcat/demo/FCat-userList.png)
![img](http://image.xfdmao.com/fcat/demo/FCat-menu.png)
![img](http://image.xfdmao.com/fcat/demo/FCat-group.png)