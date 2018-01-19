|Node.js|Express.js|Vue.js|
|--|--|--|
|7.9.0|4.16.2|2.5.13|

注：本项目指定7.9.0版本的`Node.js`，其他版本的可能不适用

### 项目简介

* 项目目的：综合性的项目提升自己的综合能力
* 本项目前端部分打包成静态文件后，可结合[另一个项目](https://github.com/wscj/fqq-backend)测试生产模式

### 效果演示（没有实时更新）
![效果演示动态图](https://github.com/wscj/static-resource/blob/master/images/fqq.gif)

### 技术栈

* 前端
	* Vue.js
	* vuex
	* vue-router
	* axios
	* sass
	* es6
* 后端
	* Node.js
	* Express.js
	* Sqlite

### 其他说明
* 新注册的用户没有好友数据，当前没有添加好友的功能，请使用已有帐号6661、6662、……、6666登录，其中6666初始化数据最完整，建议使用，密码统一为123

### 安装与运行

```bash
# 安装依赖（如果安装sqlite3失败看最后面）
$ npm i

# 预览运行，请手动在浏览器打开localhost:3000
$ npm run start

# 打包成静态文件
$ npm run build

# 调试运行
# 使用supervisor与inspect，方便后台Node.js的开发、调试
# 需要先全局安装supervisor，chrome上配置inspect
$ npm run dev
```

### 功能（整理中）

- [x] 登录
- [x] 退出登录
- [x] 注册
- [x] 下拉加载更多的动画
- [x] 展示聊天列表
- [x] 好友聊天
- [x] 展示好友分组
- [x] 等待动画
- [x] 选择提示对话框
- [x] 上传文件


### sqlite3安装失败

安装sqlite3需要的一些依赖源于不稳定的网站（国外），如果不稳定时，可以切换到[sqlite3-windows](https://github.com/wscj/fqq/tree/sqlite3-windows)分支或[sqlite3-MacOS](https://github.com/wscj/fqq/tree/sqlite3-MacOS)分支直接克隆我安装好的sqlite3文件，详见分支说明。
