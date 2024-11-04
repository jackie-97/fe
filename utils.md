直接按一位大佬给的大纲来学习即可，不要自己再写一份，这是傻逼行为，只补充它没有的东西

教程

- 低代码：https://segmentfault.com/a/1190000042810460
  - [json schema是啥](https://blog.csdn.net/xgangzai/article/details/122183483)

- 百度地图接入：https://lbsyun.baidu.com/index.php?title=jspopular

- nginx：https://juejin.cn/post/7424168473423020066?searchId=202410300856402566F5C47AD059F621B5

- debug

  - [取消勾选ignorelist](https://blog.csdn.net/qq_45024094/article/details/134964140)
  - [有时候webRoot不正确](https://blog.csdn.net/qq_45763682/article/details/130983785)，你要手动改成你的项目地址
    - ​    "webRoot": "F:/fe-projects/toucu-admin/src"

  

## elementPlus

表单校验不生效，一直判定为valid一直为true

- 



## native-ui





## pnpm







## debug

：肯定要学会debug啊，不然你线上出问题了，没法定位的



## vite



## webpack



## ci/cd





## nginx

转发与重定向区别？

- 转发是代理，客户端不用改变url
  - 如果你要访问接口，就不能用重定向，而是应该用转发
- 而重定向则是会让客户端重新访问一个新的url
  - 如果你要访问新的界面，则是用重定向



## lodash

merge

- 一般是新的替换掉旧的属性，属性类型为数组，会发生合并行为，比如object第一个元素与source的第一个元素合并掉

assign

- 从左到右，下一个对象会覆盖上一个对象



## debug

一般是选launch模式

- 除非你已经有一个再debug模式下运行的项目了

常见操作

- 在js中打断点，正常

常见问题

- 无法在vscode上打断点，一打就卡死
  - 是不是项目本身的问题？还是我配置的问题
- 断点打不准
- 断点打上了，但是无法进入

- 打了断点却出现了调试页面卡死的情况。

插件：[debugger for chrome](https://blog.csdn.net/gitblog_00257/article/details/142777978)

- 能够实现不切换到浏览器的控制台，就能直接在vscode里看变量

解决方法

- 直接写debugger，或者是在浏览器里加断点
- 
