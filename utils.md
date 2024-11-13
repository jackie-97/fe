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

- [git](https://juejin.cn/post/6974184935804534815?searchId=2024110511073927127CDF90D4B07DFB4B)

- [Element Plus版本低代码设计器FcDesigner Pro在线演示 | FormCreate](https://pro.form-create.com/view/)




## git

vscode可以方便的看对比

- 不要用git的原生工具

git 修改到一般，发现自己改错了分支，但是不想丢失这些修改

- 可以先把修改从暂存区回退到工作区

尽量减少切换分支的操作

- 

merge

- a分支合入另一个分支b的最新修改，git merge origin/b
  - 它会自动拉取操作的
- 



## elementPlus

表单校验不生效，一直判定为valid一直为true

- 

el-col可以不在el-row里面套用就可以使用

- 



form中多个item需要按规则排列

- 一般是一排4个
- 方式1
  - 在el-form下直接套用el-row，el-col即可
  - 此时不要设置inline属性，而且要

- 方式2
  - 直接设置表单组件的width，比如el-select的class="!w-240px"

- 





## native-ui





## pnpm







## debug

：肯定要学会debug啊，不然你线上出问题了，没法定位的



## vite

前端打包在做什么事情？

- 依赖解析
- 树摇
- 文件合并
- 代码切割，切割成多个chunk（块），实现按需加载
- 代码转换，es6+转成es5
- 代码压缩：主要是去除空格，空行，注释
- 源码映射，方便在调试时
- 环境变量的替换

打包与构建的关系

- 构建包括打包

打包文件bundle、代码块chunk

- 



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



## web-storage-cache

：对storage的进行了扩展，同时支持过期的功能，可用可不用



## xml-js

：用于把xml转换成object





