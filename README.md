# 基于 Vue 实战：Excel 表格上传解析和导出

## 1. 创建项目

```bash
npm install -g @vue/cli
vue create xxx

npm install less less-loader axios qs element-ui vue-router xlsx -S
```

## 2. 基本项目结构和默认代码介绍

```
|- public
    |- index.html
    |- icon.ico
    |- xxx.js / xxx.css
|- vue.config.js
|- package.json
|- src
    |- main.js
    |- router.js
    |- assets
        |- lib
            |- utils.js
        |- reset.min.css
        |- basic.css
    |- api
        |- axios.js
        |- index.js
    |- pages
        |- xxx.vue
    |- components
        |- xxx.vue
    |- App.vue

```

## 3.服务端简单介绍

技术栈：`Node + Express + MySQL`
`MySQL` 管理工具：`Navicat Premium [ˈpriːmiəm] 12`

```bash
$ node server.js
# 或者基于
$ pm2 start server.js
```

|- static
|- 打包后的项目部署在这里

## 4.安装依赖包

### client

```bash
cd ./client

npm install / yarn
```

### server

#### 安装依赖

```bash
cd ./server

npm install / yarn
```

#### 配置 mysql 环境

根目录下有 `excel.sql`文件，直接使用 mysql 可视化工具 [`navicat premium12`](https://www.navicat.com.cn/) 执行下这个数据结构文件就行，数据需要自行填充。然后启动`mysql`服务就行

[mysql 的安裝與配置](https://www.cnblogs.com/winton-nfs/p/11524007.html)

## 5.启动项目

```bash
$ cd ./client

$ yarn start
```

## 6.使用的依赖

[sheetjs](https://github.com/SheetJS/sheetjs)
[element-ui](https://element.eleme.cn/#/zh-CN/component/installation)
