本文档主要编写一些功能实现思路

教程

- awesome
  - https://github.com/pingan8787/Leo-JavaScript
  - https://github.com/csxiaoyaojianxian/JavaScriptStudy
  
- 大佬
  - https://space.bilibili.com/28696526?spm_id_from=333.337.search-card.all.click
  - [一尾流莺 的个人主页 - 专栏 - 掘金](https://juejin.cn/user/4099422807393901/columns)
    - 这个厉害了，全都有，架构师，
  
- 大全
  - https://juejin.cn/column/7064397645166411812

- 综合能力
  - 需求分析
    - https://www.bilibili.com/video/BV1rV411R72k/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4

  - 技术选型：https://www.bilibili.com/video/BV1Dx4y1E7AA/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4
  - 规划能力
    - https://www.bilibili.com/video/BV1JY4y187L5/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4
    - https://juejin.cn/post/7386089141367537705?searchId=202410271707153F704FA628D4EE7EA09F
  - 

- 基建
  - https://www.bilibili.com/video/BV1rP411f7Wn/?spm_id_from=333.337.search-card.all.click&vd_source=522153461914a766fc002cc8619314e4
- 需求文档：https://www.bilibili.com/video/BV1NY41147yW?spm_id_from=333.788.videopod.episodes&vd_source=522153461914a766fc002cc8619314e4&p=11



## 常见bug

单词拼写错误

- 比如res.forData，实际上是res.formData
- 多用ctrl+f来比对一下

打开错项目了。。。

- 

需求理解错误！

- 有时候业务缺了内容，或者是有冲突的部分，没有识别出来

设计问题

- 

样式问题

- 比如透明度
- 

遗漏

- 比如功能漏做了

数据清理的问题

- 比如做完某些操作数据没有重置

数据结构错误

- 读取：比如某些值直接就可以拿到的，你却跑到了第二层去取它
- 构造
  - 请求参数拼接错误


时序问题

- 有些数据可能晚点才能拿到，你却第一时间初始化了，相当于是把它当同步数据来弄了
  - 那么你要补充动作，做一下监听，监听它更新了的时候，你要重新调用一下方法
    - 比如位置信息可能要等1s后才能拿到，而且以prop的方式传递，然后watch即可

多个配置冲突了

- 把全部之前的能找到的配置全部清掉，再来继续开发
  - 比如nginx的配置，你有配置了转发，又配置了重定向

概念理解错误

- 你以为某个配置是默认开启的，实际上是默认关闭的，你要手动开启一下

优先级错误

- 你以为A的优先级更高，其实它被其他配置的优先级覆盖掉了

修改位置改错了

- 比如你开错了项目

数据标志位没清干净

- 比如你退出编辑了，居然还能编辑，就是
- 

数据填写错误

- 你填写了错误的数据给组件，组件会有异常行为，所以最好的做法是拷贝数据
  - 比如uniapp的map，你把经纬度数据搞反了，直接渲染出错

不可能让我前端去控制某个字段是否提交的，这是非常傻逼的操作

- 傻逼后端

业务导致

- 比如对业务不熟悉，导致做出来的功能是错的

测试功能没做好

- 测试的业务不完整，只测了相关关节的一部分。

设计问题导致

- 

公共的模块尽量不要去改

- 你在具体的业务里面做操作即可

切记不要过度封装

- 不然出了问题，要花10倍时间去解决

平时应该多测试一下主流程

- 不然主流程出问题了直接卡死



- - 






## 技巧

解决问题的方式：多选一

- 找问题根源+解决问题
  - 这种方式可能可以减少大量工作量
- 直接修复问题
  - 实在没办法，就只能直接修了

修改他人代码

- 是在原有的基础上添加
- 还是新开一个文件来开发



#### 实现技巧

多想几种不同类型的解决方案，而不是只思考同一种类型的解决方案

- 

多做可行性判断

- 比如不满足某些条件时直接return

如何获取参数？

- 通过arguments参数，多用shift方法

数据结构初始化方式

- 网络请求到数据时候前端初始化
- 表单提交后构造一下数据

要看一下某条测试数据是否具备参考性？

- 




#### 测试技巧

走一下全流程

- 很多bug就是因为你没走全流程导致的

线上调试

- 

可以先本地预览一下

- 这样可以防止你打错了包

表述问题要说清楚场景，角色

- 



#### 沟通技巧

good

- 有空看下xxx

- 可以xxx

- 我说过了xxx
  - 而不是他知道的

- 要求准确，或者是减少失误

  - 没看到，而不是没有
  - 多说应该

- 你需要多找一些解决方案

  - 不要马上就说不行
- 没事啊
  - 因为我根本不在乎


bad

- 使用反问句，难道xxx？

- 



#### 设计技巧

尽可能地去做减法

- good：先按最简单的流程，最简单的交互，先快速出一版，先运行一段时间，不满足需求了，我们再调整
- 任务本身难度是1，结果被你设计后实际难度是5或者是10
  - 一上来就是最复杂的，这就是傻逼行为，这思路本身就没法按时完工了，也是最累的

- 不要然哪些傻逼随便展示一大堆信息，前端要要查一大堆接口与字典，搞死人的
  - 应该只展示必要的信息，无关信息不要展示
    - 比如有对比的信息才需要显示
  - 至少不应该让前端去不断地查询，应该后端返必要的信息
    - 一个页面不能调用超过3个接口

不要让用户去做填空题，而应该去做选择题，

- 不然之前会有兼容性问题

值的设计应该是数字，而不是bool

- 比如目前是2个选项，未认定，已认定，后面再来个”认定中“，你就没得玩了

交互设计

- 操作指引，比如可以用图片替代的，就不要直接搞强操作指引

优先做成弹窗，而不是做成新页面

- 





## 前端综合能力

- 文档编写能力
  - 这个是一直被你忽略的，但是实际上是支柱性的能力，文档写好，一切都变得清晰
- 业务：这是最重要的，知道要有什么东西，不需要有什么
  - 熟悉开发流程
  - 熟悉常见的业务类型
  - 加强培训
    - 找项目经理或产品经理，找他们要业务培训的ppt或者是线下讲解，定期培训
- 需求分析
- 技术选型
- 规划能力
  - 工期评估
  - 风险评估&应对策略
  - 请求人力支援：比如要求来个测试
- 框架搭建能力
  - 如果叫你搭建一个项目，
- 设计能力
  - 数据结构的设计

- 代码阅读能力
  - 你一定会大量yue'du
- 工作汇报
  - 要让领导知道你做了啥
- 调试能力，也叫bug排查能力
  - 
- 善于搜索

  - 关键字：使用、入门、指南、坑
- 善于总结
  - 同样的问题，尽量不在犯第二遍
  - 多看文档，特别是[错误总结的问题](https://lbs.qq.com/faq/webFaq/jsComponent)
- 次要
  - 交互设计
    - 怎样减少用户出错，添加



开发流程？

- 比如开发分支问题，开发在dev分支，而
- 熟悉人员角色，谁是项目经理，产品经理



- 



## 开发效率

- 识别优先级，列出核心问题，砍掉次要问题
  - 先解决主要问题，次要问题砍掉或先放着，先让整体跑起来
- cv大法，不要每次都自己从头开始重写1次
  - 保留一些代码片段，比如表单验证，模态框
  - 多找一些模板项目，能够快速搭建，这样直接改一下就能用了
- 注重整体：注重某个功能整体的步骤是怎么走的！
  - 整体>>>细节
  - 你要多记流程
- 熟悉api
  - 你对api不熟悉，可能会导致很多问题
- 模仿大佬，学习好的实现习惯：看看大佬是怎么实现的，观察同事是怎么做这件事的
  - 学习他们的开发习惯
  - 学学别人优秀的设计是怎么做的，
- 做好笔记
  - 找到自己的模糊的，不熟悉的模块，捋清楚思路
  - 总结一些自己的错误开发习惯，做好避免二次犯错
  - 多写bug日记
    - 避免下次再犯
    - 多观察别人主动暴露的bug
- 提高熟练度，平时多练一下常用功能的开发，
  - 第一步就是要搭建一个好的开发环境，方便你快速测试验证
- kai'fa
- 学会找一些提效工具，或者是做一些提效工具，一定要先找，不要一上来就自己做
  - 注意不要过度追求工具，会导致投入成本过高
  - 自动化工具
    - 比如自动化打包、构建、发布
  - 做好模拟
    - 比如数据模拟，不要让
- 做好测试
  - 学习一些测试技巧，工作流
- 先做好一个完整的demo，然后再复制这个demo
  - 不要每次修改就改动一批

- 表单制作
  - 通过表单制作器，填写配置
    - 然后复制代码
  - 或通过自定义mu'ban




## 精力投入

先做好减法

- 我不打算深入前端，所以我只做通用功能
  - 基建，打包，监控，规范，微前端之类的不做，或者是不追究
  - 因为在ai时代，这些工具都会报废

- 不关注性能优化，因为很少碰到这场景
- 不打算深入后端，我后端设计能力不行的，禁不起考验

区分优先级

- 不重要的放着，或者是记录一下即可

加法

- 多往业务靠
- 多往管理和设计靠





## 需求分析

：目标都是如何做好

- 实现要了解项目业务，这样你才能识别伪需求，才能减少被傻逼带坑里的次数
- 先熟悉整体流程，想要达成什么效果？
- 明确客户想要达成的预期效果
  - 也要识别可行性与风险
- 然后确认需求的优先级
  - 把不必要的功能靠后实现或者是砍掉
- 一定要多问，多确认，这样才能减少浪费的人工

- 加强团队沟通，特别是产品经理，明确需求优先级
  - 同时做好记录，防止耍赖
- 学会编写需求文档：PDR
  - 为啥要有文档？因为如果你啥文档都不写，那就是任由老板乱来咯，乱定时间咯
- 学会编写用户故事
- 收集反馈
  - 根据反馈调整需求
- 主动识别



## 技术选型

：解决问题是哪些场景下应该选什么技术的问题

考虑因素

- 需求：选的技术是否满足功能，性能方面需求
- 开发、维护成本：时间成本，是否难以集成，是否有说明文档
- 安全性：这个问题一般不用考虑
- 生态：生态很差，出了问题压根没法解决的
- 兼容性：看跨平台的能力如何

需要准备一些东西

- 比如申请账号之类的，比如百度地图

反面

- 选了cocos作为前端开发注定要被坑死，效率非常拉跨



## 规划能力

#### 开发排期

参与角色

- 项目经理（一般是他或者是产品经理来排期的）
- 开发者

流程

- 要对着设计页面，比如蓝湖来制定开发计划

  - 一般是安排最近一周的任务


- 划分的单位可以搞大一些，不要太关注细节


- 









## 常用代码片段



## 技术选型

：这个其实小问题



## 实现逻辑

判定一个条件，还是需要判断多个条件

- 有时候看似只需要判断多个，实则只需要判断一个条件

一般是取&&操作，比如

- 



## 阅读他人代码

- 要文档
- 通过阅读一个一个小案例
- 通过debug
- 
- 



## 工作流

- 搞清楚开发分支，生产分支是哪个
  - 一般是dev开发，prod生产

分支管理

- feature/aaa,feature/bbb，就可以开发新的功能
- dev
  - feature分支开发完就可以合并到dev
- prod
  - dev上验证完就可以合入到prod
- hot-fix
  - prod出问题了，就可以热修复一下

合入流程

- 



#### uniapp工作流

测试

- 要结合微信开发者工具



#### 线上bug处理

- 直接把上一个前端打的包丢上去，先让用户看着
- 前端代码不用回滚，直接在hot-fix分支就修改即可，修改完之后本地验证一下，合入到prod，然后通过后直接打包给线上验证，验证通过后你再合入代码
  - 即打包在前，代码合入在后



#### 分支管理

为了防止遗漏更新

- 需要每个分支都合入一下到dev或者是prod，如果你忘记了



## 问题

为啥不做后端？

- 因为我目前没法保证数据的完整性
- 还有不会数据修复
- 设计能力未曾锻炼。

计算中的模态有啥特点？

- 中断性，你必须要与模态框内容交互才能继续，你没法操作其他内容
- 命名由来：表示特定的一种交互方式，与名称本身并非强关联
