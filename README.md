# vue-nuxt

> Nuxt.js project
> 服务端渲染框架，接口请求使用axios标配

## Build Setup

``` bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm start

# generate static project
$ npm run generate
```

## 部署服务端流程
``` bash
# 项目打包以后，npm run build，将下面的几个文件放到服务器
  .nuxt
  static
  nuxt.config.js
  package.json
  
$ 运行npm install 安装package里的依赖
$ 运行npm start 就可以运行起来nuxt的服务渲染了  
$ 最好用pm2做管理
[nuxt部署流程](https://segmentfault.com/a/1190000014450967)
```

Nuxt例子请查看： [Nuxt.js docs](https://nuxtjs.org).
