# generator-loopback-vue [![Build Status](https://travis-ci.org/qxl1231/generator-loopback-vue.svg?branch=master)](https://travis-ci.org/qxl1231/generator-loopback-vue)

## 通过本源码你可以学习到:[![CircleCI](https://circleci.com/gh/qxl1231/generator-loopback-vue.svg?style=svg)](https://circleci.com/gh/qxl1231/generator-loopback-vue)
- Strongloop是是如何通过一行命令和代码实现restful API接口,包括CRUD等14个接口
- model是如何定义的,以及model-relation 定义,以及ACL接口权限控制等
- CI持续集成的配置,Docker容器,docker部署文件
- **如何登录鉴权,以及接口权限控制**
- vue1.0 是如何玩?以及vue-resouce的使用,vue-router,webpack,babel等
- loopback自带的authenticate 权限控制,accesstoken机制,credentials
- strong-pm 部署命令,以及slc主要命令
- 如何把项目部署在daocloud中,以及集成daovoice服务
- ***增加了个vue-pagenav 组件的使用 实现分页功能***


## Docker镜像 ,在daocloud.io中
最新版本: latest
镜像地址: daocloud.io/qxl1231/lb-vue2

## 在线demo:
> http://loopback-vue.daoapp.io/
`帐号:test,密码:testpwd`

## 部分截图
![image](https://cloud.githubusercontent.com/assets/8305742/17387903/810c8b16-5a2a-11e6-862a-9306067bfc34.png)
> 集成了daovoice玩玩哈哈~~~炫酷!
![image](./daovoice.png)

![image](https://cloud.githubusercontent.com/assets/8305742/17387949/dce5d7d0-5a2a-11e6-9e1d-5fe93b2924b2.png)

The project is generated by [LoopBack](http://loopback.io).+[vue.js](http://vuejs.org).

## 如何启动:(国内用cnpm(先运行npm i cnpm -g),国外用npm)
```   
       1. npm i   
       2. 修改datasources.json 中的数据库配置比如:localhost:27017
       3. node server/bin/create-admin.js 添加管理员帐号,密码
       3.npm run build:js & node .(cold reload) --hot reload npm run watch:js
```

## 遇到问题1:loopback+vue 不能运行
答:1.npm install   2.npm run build:js  3.node .

## 问题2:热部署
To use hot reload, please try this command:npm run watch:js & node .

## 热启动:$npm run watch:js & node .

 
## 问题3:If you have error, try this:
回答:
` npm install
  vueify-insert-css vue-hot-reload-api
  babel-core babel-preset-es2015
  babel-plugin-transform-runtime babel-runtime@5
  --save-dev `
 
  
## Hot reloading detail: 
https://github.com/vuejs/vueify

## 其他help===>loopback 常用命令行:
 - slc loopback 初始化项目
 - slc loopback:datasource
 - slc loopback:model
 - slc loopback:relation
 - slc loopback boot-script


## others:deploy and status

 - slc deploy http://usr:pwd@localhost:port  
 - slpmctl -C http://usr:pwd@localhost:8701 ls   

 - slpmctl -C http://usr:pwd@domain:8701 status 

 - pm2 start -n weather app.js

 - pm2 start -n app_update_server server.js

## LICENSE

MIT



## 捐赠

您的捐赠，是我持续开源的动力。

支付宝 | 微信
------|------
![](./alipay.jpeg) | ![](./Wechat.jpeg)
