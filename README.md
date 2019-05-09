
采用全新的前后端分离模式，本仓库代码中已集成前端vue打包后文件，可免去打包操作

如需调整前端代码，请单独下载前端代码，前端代码在根目录的ux文件夹中

## 主要技术栈

后端框架：ThinkPHP 5.0.2

前端MVVM框架：Vue.JS 2.5.x 

路由：Vue-Router 3.x 

数据交互：Axios 

UI框架：Element-UI 2.6.3 

悟空crm9.0的运行环境要求PHP5.6以上


## 一键安装

代码中已集成前端vue打包后文件，可免去打包操作：
以本地（phpstudy集成环境）搭建举例：
下载悟空CRM9.0开源版，在服务器根目录（www目录）下创建72crm文件夹，并放置代码； 浏览器访问

`http://localhost/72crm/index.php/admin/install/index.html `

根据安装提示步骤，完成悟空CRM9.0 的部署安装





## 开发依赖（需个性化安装或调整前端代码请按照以下教程，一键安装用户可忽略）

### 数据交互 
数据交互通过axios以及RESTful架构来实现 
用户校验通过登录返回的auth_key放在header 
值得注意的一点是：跨域的情况下，会有预请求OPTION的情况

### Server搭建 
服务端使用的框架为thinkphp5.0.2，搭建前请确保拥有lamp/lnmp/wamp环境。

这里所说的搭建其实就是把server框架放入WEB运行环境，并使用80端口。
导入服务端根文件夹数据库文件public/sql/5kcrm.sql，并修改config/database.php配置文件。

### 配置要求
PHP >= 5.6.0 （暂不支持PHP7及以上版本）
当访问 http://localhost/, 代表后端接口搭建成功。
### 前端部署
安装node.js 前端部分是基于node.js上运行的，所以必须先安装`node.js`，版本要求为6.0以上

使用npm安装依赖 下载悟空CRM9.0前端代码； 可将代码放置在后端同级目录frontend，执行命令安装依赖：

    npm install

修改内部配置 修改请求地址或域名：config/dev.env.js里修改BASE_API（开发环境服务端地址，默认localhost） 修改自定义端口：config/index.js里面的dev对象的port参数（默认8080，不建议修改）

### 运行前端

     npm run dev

注意：前端服务启动，默认会占用8080端口，所以在启动前端服务之前，请确认8080端口没有被占用。
程序运行之前需搭建好Server端



## 系统介绍

以下为CRM9.0 部分功能系统截图



![](https://github.com/72crm/72crm/blob/master/ux/intro_img/g1.png)
![](https://github.com/72crm/72crm/blob/master/ux/intro_img/g2.png)
![](https://github.com/72crm/72crm/blob/master/ux/intro_img/g3.png)
![](https://github.com/72crm/72crm/blob/master/ux/intro_img/g4.png)
![](https://github.com/72crm/72crm/blob/master/ux/intro_img/g5.png)
![](https://github.com/72crm/72crm/blob/master/ux/intro_img/g6.png)
![](https://github.com/72crm/72crm/blob/master/ux/intro_img/g7.png)
![](https://github.com/72crm/72crm/blob/master/ux/intro_img/g8.png)
![](https://github.com/72crm/72crm/blob/master/ux/intro_img/g9.png)
![](https://github.com/72crm/72crm/blob/master/ux/intro_img/g10.png)





