本文档主要编写一些功能实现思路

教程

- 常见功能
  - https://juejin.cn/post/7088144745788080142?searchId=202410271635456BBE16F0D81AB48A17CF
- 优秀项目：https://doc.iocoder.cn/video/
- 地图接入
  - uniapp
    - 使用腾讯地图获取定位：https://juejin.cn/post/7202149834363142201#heading-7
    - https://blog.csdn.net/abs625/article/details/138908945
    - https://blog.csdn.net/qq_25430563/article/details/109818716
    - key配置：https://blog.csdn.net/SOLar7SysteM/article/details/123856915
    - demo:https://www.zeeklog.com/uni-app-wei-xin-xiao-cheng-xu-zhong-guan-yu-map-di-tu-shi-yong-an-li-fen-xiang/



## 项目模板

vue

- [视频教程 | ruoyi-vue-pro 开发指南](https://doc.iocoder.cn/video/#大纲)
  - 基于elementPlus
- [naive-ui-admin](https://github.com/jekip/naive-ui-admin)
  - 基于naive-ui

uniapp

- 



## 数据大屏



## 响应式



## 滚动加载内容



## 地图接入

地图坐标有很多标准

- 常用国测局坐标





#### 百度地图接入到vue

：通过插件[vue-baidu-map-3x](http://map.heifahaizei.com/doc/begin/install.html)

百度地图文档：

常见

- 获取用户坐标
- 地址解析与逆地址解析
  - 要先获取解析器对象，然后再

- 绘制多边形区域
  - 绘制
  - 编辑
  - 显示
  - 获取实体点的信息
- 控制地图的缩放，通过滚轮
  - 设置属性即可

- 根据多边形自动计算地图中心点和缩放比例
  - 需要自己计算，获取所有4个顶点，然后计算出中心点


能否主动获取多边形上的所有点？目前是只能移动点位的时候获取

- 

多边形新建的时候

- 要不要做一些控制操作？比如不能编辑其他的多边形

新建多边形时，隐藏其他多边形

- 直接重置shu'ju

为啥添加点的时候就会自动绘制多边形？

- 因为修改了数据，bm-polygon组件的path值修改了，就会重新渲染
  - 而不是主动调用绘制操作！

标记物不显示

- 其实是显示了，只是你的给的错了，所以它显示在别处了，
- 用组件方式来渲染



#### 腾讯地图接入到uniapp

地图厂商要我们自己选还是会自动计算出来？

- map组件会自动根据平台计算出来，到底是选哪个地图作为实现

我怎么确定要不要付费？

- 

我怎么知道要申请1家，还是多家的地图账号

- 目前只用到微信小程序，那就只申请腾讯地图

流程

- 注册腾讯地图账号
- 授权给对应的小程序
- 请求方式
  - 要么限制ip
  - 要么通过签名方式调用
    - 这个比较麻烦
  - 不限制
    - 偷懒的话

地图无法渲染

- 可能是小程序没有添加安全域名导致的，但是我现在是web端啊
- latitude与longitude的值给错了，你写反了，导致地图渲染为灰色



## 字典实现

常见操作

- 存储
- 读取某个属性

目标

- 有效的存储字典
- 方便取出



## 组件封装

组件拆分，哪些部分可以拆分成组件，哪些可以不拆的

- 



## 审批业务



## 表单低代码

快速生成表单



## 问题

获取实例的方式？

- 通过new
- 通过工厂方法，即静态方法
- 通过hook，usexxx
  - vue、react中很常见
- 通过回调中获取
- 通过访问属性
- 通过Object.create
- 反序列化JSON.parse



初始化数据的方式？

- 通过生命周期函数来完成初始化
- 还是在具体的方法里面再来初始化？



功能实现方式

- 组件
- 方法