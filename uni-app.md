uniapp也有做，真的是醉了

教程

- [入门](https://juejin.cn/post/7248835844659839033?searchId=20241030092715F11BDF24DA2ECFD97019)
  - https://zh.uniapp.dcloud.io/tutorial/debug/debug-web-via-hx.html

- ui库
  - 有内置组件
  - 还有[uni-ui](https://zh.uniapp.dcloud.io/component/uniui/uni-ui.html)
  - 还有[uview](https://www.uviewui.com/components/intro.html)

- 




## 关键

工作流是怎样的？

- 



## 问题

uniapp的工作流是怎样的？是在vscode里面编辑吗？然后跑到uniapp里面进行打包？

- 其实uniapp本身也不错的
- 是要打开微信小程序开发者

如何启动项目？

- 安装插件
- 然后启动到浏览器

我用uniapp开发微信小程序，应该用uniapp的api还是微信小程序的原生api？

- 基本只用uniapp的api，除非有它没封装的api，采用原生的api

uniapp开发只用普通浏览器测试，能够完整测试它的能力吗？

- 

uniapp为啥会有项目类型？

- 我理解的就是一种项目类型

uniapp web项目不支持运行到小程序

- https://ask.dcloud.net.cn/article/35878

从hbuilder打开微信开发者工具失败

- 服务端口要打开
- 还有

微信的开放能力比如wx.switchTab是否只能在微信开发者工具或者是真机才能生效？还是在普通浏览器上也能生效？

- 只能在前两者生效，普通浏览器不能生效



这三个ui库有啥区别？

- 内置组件不用另外安装
- uni-ui是官方出的
- uView不是官方出的，但是做的很不错

uniapp居然支持下载完马上就打开文件

- 通过下载成功的回调，拿到地址res.tempFilePath，调用openDocument就可以打开咯
