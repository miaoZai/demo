# 声明·感谢：
本模块大部分内容来自<a href="https://github.com/Advanced-Interview-Question/front-end-interview" target="_blank">《前端面试与进阶指南》—— xiaomuzhu</a>，
特别感谢xiaomuzhu。


## 模块概览

本项目会分为七大模块，分别为：前端基础、框架解读、工程化、性能优化、计算机基础、Typescript、细分领域。

### 前端基础

这一部分以JavaScript、CSS、HTML这前端传统的三剑客为主，以浏览器原理等为辅，这一模块的构成不是简单得采用罗列面试题+罗列对应答案的方式，我们首先会区分重难点和非重点知识,再进行相应的解读。

对于非重点或者简单的知识我们采用罗列答案的方式，这一部分主要是帮助开发者快速过一遍这些内容，比如『==和===的区别是什么？』这种问题属于简单型的问题，我们只会做简单的解答，并不会深入历史讲清楚『===』诞生的原因、背后原理之类的。

对于重点和难点知识，我们会会提供两个版本的解读，简略版本会直接罗列相关要点，如果对相关知识已经掌握，可以快速阅读简略版作为快速地复习，详细版会针对相关知识进行深度解读，如果对相关知识不够了解，那么建议阅读详细版。

### 框架解读

框架部分一般分为两种，一种是框架原理知识，一种为实战技巧。

#### 框架原理

框架原理是必考的内容，因为没有公司希望招一个API小子过来，在这部分我们跟『前端基础』中的重点部分处理方法一样，通过详略两个版本的内容。

我们不会通过罗列源码的方式进行原理讲解，我们会尽量简化代码做到深入浅出。

#### 实战技巧

实战技巧主要涉及基础组件实现，考察是否只会用现成组件库，有没有造组件轮子的能力。

我们会对常见的基础组件实现,创建一个对应的实战项目，毕竟这些实战技巧脱离了项目只靠罗列答案，稍微有较深入的追问就原形毕露。

### 工程化

前端工程化现在已经成为标配了，我们目前计划的内容有：webpack、Babel、Git、测试、Node工具。

#### webpack

webpack是前端项目的事实上的打包标准，这部分我们会从打包原理、插件loader编写和实战搭建三个部分进行讲解。

webpack的知识是实战型的，所以会有一个实战源码。

#### Babel

Babel也是前端事实上的转译标准，不过这部分要考察的内容并不多，基本就是插件的编写和编译原理，我们也会有对应的实战源码。

#### Git

Git是任何软件工程师的必备技能（SVN瑟瑟发抖），这部分主要讲两个部分：工作流和使用技巧。

#### 测试

测试是软件工程的必备，但是在前端领域至今的重视程度不够，我们看到招聘市场上对测试的要求也不多。

但是测试是软件工程的基本要求，我们还是增加了这个部分，主要是对测试工具的对比和入门，以及测试思想的解读。

#### Node工具（todo）

实际上Node才是前端工程化的基石，现在前端对Node要求也越来越多，当然除了写中间层之外，一大用处就是造基于Node的工程工具，如下：
![2019-06-12-17-52-29](https://xiaomuzhu-image.oss-cn-beijing.aliyuncs.com/998be8184d459d6592b2a2cacd10380b.png)

这个部分我们会造一个基于Node的Cli工具，并将各种代码美化工具、代码检测工具以及各种工程化的思想集成进去，除了学会造node工具之外，对前端工程化的知识算是一个总的梳理。

### Typescript（未完成）

考虑再三，我还是认为TS应该占据一席之地，这两年Typescript其实有成为前端大型项目的标准开发语言，Angular这种庞然大物早就用了TS自不必说，Vue已经抛弃flow用TS重写（用过flow就知道多难用），甚至连Facebook开源的jest也抛弃flow改用TS，在Node后端框架中最流行的Nestjs也是基于TS的，还有vscode、antd、rxjs等等都是基于TS的。

在招聘信息上我见到越来越多的要求是『有使用Typescript的经验者优先』这种条件，个人认为在Vue 3.0正式发布后TS会逐渐成为硬性要求，虽然尤小右声明Vue在使用层面不限制js或者ts，但是Angular团队也是这么说的。。。但是问题在于Vue的生态会逐渐被TS重写，Vue对TS的支持会非常好，会有越来越多的团队用TS开发Vue新项目，这个趋势是不可逆的，包括本身对TS支持良好的Angular和React，三大框架都被TS纳入版图之后，这个方向已经很明朗了。

所以，这部分会介绍TS的基本语法和高级类型编程，然后用TS重写一个库作为实战。

### 性能优化

性能优化是任何软件工程必备的步骤，我们不会罗列雅虎军规，而是进入到实战进行优化。

这个部分我们不会罗列任何东西，会直接拿一个项目进行一步步的优化，原因很简单，性能优化就是与实战强相关的，脱离实际谈优化都是空中楼阁，在面试过程中有没有进行过实际优化，如果没有实战作保证很容易翻车。

### 计算机基础

计算机基础是前端面试近两年的考察重点，也其中算法涉及的最多，所以这部分的重点在于算法。

另一个重点是网络部分，HTTP协议也是必不可少的。

这部分会分为这几个部分： 数据结构、算法、网络。

操作系统，数据库和编译原理部分暂时没有，前端涉及的编译原理主要是编译原理的前端部分，在『工程化』模块中的babel会讲到相关知识，而前端的操作系统其实是浏览器，这部分在『前端基础』模块会涉及，数据库的应用场景在前端很有限，基本以数据类的重型前端项目为主，这个部分暂时没有考虑加。

### 细分领域（todo）

前端的目前分化的领域大概有四类：移动前端、可视化、图形、Node。

移动web前端,他们大部分时间在为移动设备工作,除了传统前端知识外,还需要运用 hybrid、RN 甚至一些 native 技术
![移动前端招聘信息]( https://xiaomuzhu-image.oss-cn-beijing.aliyuncs.com/5efdb218b01fbe5842a03131db64eddf.png)

可视化前端,他们大部分时间再跟数据、canvas、svg 等打交道，需要一定的可视化科学的基础和相关领域算法
![数据可视化招聘]( https://xiaomuzhu-image.oss-cn-beijing.aliyuncs.com/af0f1a1d78a9216a177d8725825f17e0.png)

图形互动前端，他们离传统意义的前端更远，大部分时间在处理图形学范畴的东西
![图形互动]( https://xiaomuzhu-image.oss-cn-beijing.aliyuncs.com/1935882f80633f14b9214fdaf026ede1.png)

Node 前端,讲道理 node 工程师跟前端的关系已经很小了,但是也挂了前端的头衔,他们的技术要求基本就是个后端,除了也用 js
![Node 前端]( https://xiaomuzhu-image.oss-cn-beijing.aliyuncs.com/bfe816f0325b3b466e1dea9aacd90b5a.png)

实际上，这四个领域的分化导致其对特定领域的知识要求更高，而相关的资料就相比于通用前端知识更少，这部分应该是本项目难度最大的地方，我会按照移动前端、Node前端、可视化、图形先后顺序进行更新，这也是我个人的熟悉程度，也是目前市面上相关需求的大小排序，毕竟市场对于找一个写shader的前端需求有限，一般是一些大厂或者游戏厂商。