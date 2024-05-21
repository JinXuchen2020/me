---
title: 在线Excel编辑系统
---
 此项目是基于[UniverJs](https://github.com/dream-num/univer/)框架搭建的在线Excel编辑系统, 集成了微信登录, 实现了在线Excel的编辑、保存、导入和导出功能。项目预览地址：[在线Excel](https://www.hlchangrun.top/).

## 项目介绍

### 业务需求

在线Excel编辑系统主要是为企业内部人员解决了以下几个问题：

1. 采用微信登录，让内部人员可以随时随地编辑自己的Excel表格。
2. 内部人员可以独立编辑、保存自己的Excel表格，不用担心数据丢失和混淆。
3. 管理人员可以随时查看和管理所有员工的Excel表格，并提出更新意见。保证数据的正确性和完整性。
4. 管理人员可以导入、导出Excel表格，并将其分享给其他人员。

### 技术选型

前端技术栈：

1. 框架：UniverJs + React + Vite + Typescript
2. UI组件库：UniverJs + Ant Design
3. 数据处理：luckyexcel + Exceljs + UniverJs

后端技术栈：

1. 框架：Node.js + Express
2. 微信登录：Wechat-js-sdk

## 项目架构

### 前端架构

1. 框架：采用UniverJs + React + Typescript + Ant Design实现。
   1. 将UniverJS封装为React组件，并通过props传递数据，根据数据来实现Excel表格的渲染。
   2. 实现自动保存功能，当用户关闭表格时，自动保存当前的修改，防止数据丢失。
   3. 通过添加自定义UniverJS插件，实现手动保存功能。
2. 导入导出功能：采用luckyexcel + Exceljs + UniverJs实现。
   1. 利用luckyexcel实现Excel表格的导入
   2. 利用Exceljs实现Excel表格的导出
3. 微信登录：采用Wechat-js-sdk实现。
   1. 将微信登录功能封装为React Hooks，方便复用。
   2. 当用微信内置游览器登录时，自动获取用户信息，并读取该用户的Excel表格数据。
   3. 当用外部浏览器登录时，跳转到微信扫码登录页面，用户扫描二维码登录后，获取用户信息，并读取该用户的Excel表格数据。
   4. 利用SessionStorage缓存用户信息和Token，Token过期需在登录。
4. 部署：采用Github Actions编写CI/CD流程, 实现自动部署, 测试版部署到github pages，正式版部署到云服务器。

### 后端架构

1. 框架：采用Node.js + Express实现。
   1. 实现微信登录功能，获取用户信息，并读取该用户的Excel表格数据。
   2. 微信登录后，利用JWT生成Token，实现用户认证。
   3. 实现Excel表格的CRUD操作，包括创建、读取、更新。
3. 部署：采用Webpack进行打包，在服务器上启动Node，运行Express服务。

## 项目进度

- [&#x2714] 前端架构设计
- [&#x2714] 后端架构设计
- [&#x2714] 微信登录功能实现
- [&#x2714] 导入导出功能实现
- [&#x2714] 自动保存功能实现
- [&#x2714] 手动保存功能实现
- [x] 项目部署
- [x] 项目测试
- [x] 项目上线
  

## 项目总结

此项目功能相对简单，总体难度不大，但还是遇到几个问题：

### 实现Excel导入、导出功能

在项目中，因为需要将导入的Excel表格转换为UniverJS可识别的格式，所以找到了luckyexcel这个库，该库实现了Excel格式转换为UniverJS可识别的格式，但没有实现Excel的导出功能，需要自己实现。所以有去找到了ExcelJS库，实现了UniverJS格式到Excel格式的转换，最终实现了Excel的导出功能。

### 实现保存功能

在项目中，使用了两种方法来实现保存功能。

第一种方法是使用在表格关闭时，自动保存当前的修改，防止数据丢失。

第二种方法是编写UniverJS的插件，添加手动保存按钮，用户点击按钮时，保存当前的修改。

这两种方法的实现代码相似，但第二种方法需要将更新的数据传递给UniverJS插件，并触发UniverJS的保存功能。

~~~bash
constructor(
  private _config: any,   // 接收传递的数据，且必须在第一位
  // inject injector, required
  @Inject(Injector) override readonly _injector: Injector,
  // inject menu service, to add toolbar button
  @Inject(IMenuService) private menuService: IMenuService,
  // inject command service, to register command handler
  @Inject(ICommandService) private readonly commandService: ICommandService,
  // inject component manager, to register icon component
  @Inject(ComponentManager)
  private readonly componentManager: ComponentManager
) {
  // plugin id
  super();
}
~~~

### 编写登录功能React hooks, 实现登录状态的统一管理

登录功能的hook主要实现了一下功能：

1. 登录：处理微信SDK返回的Code，实现微信登录，获取用户信息，并缓存。
2. 登录状态：根据SessionStorage的缓存信息，判断用户是否登录。
3. 登出：清除SessionStorage缓存的用户信息和Token。

### 实现微信登录的流程

微信登录的实现，因为要求回调的域名必须是公网可访问的，所以造成实现的过程比较复杂，主要分为以下几个步骤：

1. 在[微信开放平台](https://open.weixin.qq.com/)注册账号, 并完成实名认证。
2. 创建网站应用
   1. 购买云服务器、域名、CDN等服务。
   2. 申请ICP备案。
   3. 填写微信开放平台网站登记表。
3. 待定

### 后端打包配置

因为后端时采用Typescript的编写的，所以打包时做了一些额外的配置：
1. 入口文件
  ~~~bash
  entry:'./bin/server.ts'
  ~~~
2. 文件编译
  ~~~bash
  module : {
    rules: [
      {
        test: /\.ts?$/,
        exclude: /node_modules/,
        use: {
          loader: 'ts-loader'
        }
      }
    ]
  },
  ~~~
3. 静态文件复制
  ~~~bash
  plugins: [
    new copyPlugin({
      patterns: [
        { from: 'public', to: __dirname +'/dist/public' }
      ]
    })
  ]
  ~~~
4. 环境变量设置
  ~~~bash
  plugins: [
    new DefinePlugin({
      'process.env.ADMIN_USER_ID': JSON.stringify(process.env.ADMIN_USER_ID)
    })
  ]
  ~~~
6. 输出文件
  ~~~bash
  output: {
    filename: 'bundle.cjs',
    path: __dirname +'/dist/server'
  },
  ~~~

### 后端部署

后端的部署有两种选择：

1. 本地部署：将nodejs免安装版和后端打包文件一起打包，复制压缩包到本地并解压，然后在本地启动Node服务，运行Express服务。
2. 云服务器部署：待定。
