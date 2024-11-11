直接按一位大佬给的大纲来学习即可，不要自己再写一份，这是傻逼行为，只补充它没有的东西

教程

- vue
  - https://juejin.cn/post/7164159759619194893?searchId=2024102917184027ADB219F9CC5FA8709E
  - https://juejin.cn/post/6940454764421316644?searchId=2024102917184027ADB219F9CC5FA8709E

- 



toRef

- 把响应式对象的某个属性，变成单独的响应式对象，同时保持与之前的链接



[toRefs](https://cn.vuejs.org/api/reactivity-utilities.html#torefs)

- 套用了toRefs，可以保证对象被解构后依旧是响应式的
- 防止直接结构，丢失了响应性



## hook

多做一些hook的练习

useXXX都是返回函数或者是响应式数据

- 比如useState



## pinia

useXXXstore，调用后返回的是单例的store

- 



## 问题

响应式是啥？

- 是指数据与视图同步

如何给reactive函数生成的对象整体赋值？

- 改成ref来实现
- 用Object.assign实现

计算属性依赖于

- 另一个属性响应式属性，能够监听到异步数据的更新

- 
