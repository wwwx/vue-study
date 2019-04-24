## vue介绍

   Vue.js是一个轻巧、高性能、可组件化的MVVM库，同时拥有非常容易上手的API；

   Vue.js是一个构建数据驱动的Web界面的库。

###  官方介绍

> Vue.js（读音 /vjuː/，类似于 **view** 的读音）是一套构建用户界面(user interface)的**渐进式框架**。与其他重量级框架不同的是，Vue 从根本上采用最小成本、渐进增量(incrementally adoptable)的设计。Vue 的核心库只专注于视图层，并且很容易与其他第三方库或现有项目集成。另一方面，当与[单文件组件](https://vue.docschina.org/v2/guide/single-file-components.html)和 [Vue 生态系统支持的库](https://github.com/vuejs/awesome-vue#components--libraries)结合使用时，Vue 也完全能够为复杂的单页应用程序提供有力驱动。



关键词： MVVM框架、数据驱动、组件化、轻量、简洁、高效、快速、模块友好



### **渐进式框架Vue**

渐进式我个人理解就是阶梯式向前。vue是轻量级的，它有很多独立的功能或库，我们会根据我们的项目来选用vue的一些功能。

vue的渐进式表现为：

> 声明式渲染——组件系统——客户端路由——-大数据状态管理——-构建工具

我们开发项目时如果只用到vue的声明式渲染，我就只用vue的声明渲染，

而我们要用他的组件系统，我们可以引用它的组件系统。 

单页面应用程序时往往是需要路由，这时候需要把vue的插件（vue-router）拉进来做路由，

如果我们的项目足够复杂，大量的使用组件而且难以去管理组件的状态，这个时候我们使用vue-resource,vue-resource是集中来管理我们的状态的。

项目完成后需要构建工具来build我们的系统，来提高我们的效果，最后形成完成的项目。

https://mp.weixin.qq.com/s/3BukYO35vd7a0d-iMXZinw

### vue中两个核心点

**1.响应式数据绑定** 
当数据发生变化是，vue自动更新视图 
它的原理是利用了 [Object.definedProperty](http://blog.csdn.net/webxiaoma/article/details/72801538) 中的setter/getter 代理数据，监控对数据的操作。（这也是为什么vue不支持ie8 以及更早的ie浏览器的原因）



**2.组合的视图组件**

- ui页面映射为组件
- 划分组件可维护、可重用、可测试



### **虚拟DOM**

js的运行速度已经很快了，然而大量的DOM 操作就会变得很慢，

Vue的编译器在编译模板之后，会把这些模板编译成一个渲染函数 。

而函数被调用的时候就会渲染并且返回一个 虚拟DOM的树 。

这个树非常轻量，它的职责就是描述当前界面所应处的状态。

当我们 有了这个虚拟的树之后，再交给一个patch函数，负责把这些虚拟DOM真正施加到真实的DOM上 。

在这个过程中，Vue有自身的响应式系统来侦测在渲染过程中所依赖到的数据来源。

在渲染过程中，侦测到的数据来源之后，之后就可以精确感知数据源的变动。

到时候就可以根据需要重新进行渲染。

当重新进行渲染之后，会生成一个新的树，将新树与旧树进行对比，就可以最终得出应施加到真实DOM上的改动。

最后再通过patch函数施加改动。



![](https://img-blog.csdn.net/20170215095002326)



![www](https://img-blog.csdn.net/20170604175120514?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvd2VieGlhb21h/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

### **MVVM模式**

可能你经常听说MVC 模式 和MVVM 模式。
angular 就是所谓的 MVC 模式的框架，model 、view、controller。
而vue 是 MVVM 模式的框架，即
M： model （数据层，也就是指数据（前端是js））
V：  view ( 也就是指DOM层 或用户界面 )

VM : view-model (处理数据和界面的中间层，也就是指Vue)

![](https://img-blog.csdn.net/20170604180151326?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvd2VieGlhb21h/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)



### 应用场景

- [ ] 构建完整 SPA

- [ ] 与服务器端一起使用

  



### vue基础知识

https://vue.docschina.org/v2/guide/index.html

API  https://vue.docschina.org/v2/api/



### vue全家桶

vue + vue-router + vuex + axios  + vue-cli



### UI框架

PC:  element-ui,  antd  ...

移动端： mint-ui  , vant,   yd-ui  ... 



### 性能优化





### 前端资料

印记中文 https://docschina.org/

前端九部 https://www.yuque.com/fe9/basic/ntcuf1

掘金 https://juejin.im/   

MDN https://developer.mozilla.org/zh-CN/docs/Web