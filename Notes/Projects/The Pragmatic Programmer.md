<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [The Pragmatic Programmer](#the-pragmatic-programmer)
  - [注重实效的哲学](#%E6%B3%A8%E9%87%8D%E5%AE%9E%E6%95%88%E7%9A%84%E5%93%B2%E5%AD%A6)
    - [软件质量与维护](#%E8%BD%AF%E4%BB%B6%E8%B4%A8%E9%87%8F%E4%B8%8E%E7%BB%B4%E6%8A%A4)
    - [进步和沟通](#%E8%BF%9B%E6%AD%A5%E5%92%8C%E6%B2%9F%E9%80%9A)
  - [注重实效的途径](#%E6%B3%A8%E9%87%8D%E5%AE%9E%E6%95%88%E7%9A%84%E9%80%94%E5%BE%84)
    - [避免重复](#%E9%81%BF%E5%85%8D%E9%87%8D%E5%A4%8D)
    - [正交性](#%E6%AD%A3%E4%BA%A4%E6%80%A7)
    - [可撤销性](#%E5%8F%AF%E6%92%A4%E9%94%80%E6%80%A7)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

## The Pragmatic Programmer

### 注重实效的哲学

#### 软件质量与维护

> Provide Options, Don't Make Lame Excuses

提供选择而不是借口，不要说做不到，要说明能够做什么来挽回局面

> Don't Live with Broken Windows

“破窗”见一个修一个。就算再没有时间，也要思考破窗的解决方案，留下注释，指定解决计划和日期。将破窗处于自己的掌控之中

> Make Quality a Requirements Issue

  - 让质量成为需求。

要学会在质量和发布时间之间做出权衡。如果你给用户某样还用的过去的东西，让他们及早使用，他们的反馈常常会把你引向更好的解决方案

  - 知道何时止步

不要因为过度修饰和过于求精而摧毁完好的程序：因为它不可能完美。与其过度修饰，不如思考正确的体验和需求

#### 进步和沟通

> Invest Regularly in Your Knowledge Portfolio
> 定期为自己的知识资产投资

> Critically Analyze What You Read and Hear
> 批判的分析自己所看见的和听见的

> It's Both what You Say and the Way You Say It
> 说什么和怎么说一样重要。

没有有效的交流，一个好想法也只是个没人要的孤儿。

只有当你在传达信息，并正确的传达给对方的时候，才是一次真正的交流。在那之前思考这些问题：

  - 你想让他们学到什么？
  - 他们对你讲的什么感兴趣？
  - 他们有多少经验？
  - 他们想要多少细节？
  - 你想让谁拥有这些信息？
  - 如何促使他们听你说话？

让听众参与，做倾听者：如果你想让别人听你说话，那么要先听他们说话

### 注重实效的途径

#### 避免重复

> DRY - Don't Repeat Yourself

关于复用组件和UI/逻辑分离这方面，可以学习React/ReactNative

注意元素之间的相互关联，使用推导来尽量避免不必要的重复

> Make It Easy to Reuse
> 尽量复用

#### 正交性

正交性：不相依赖性/解耦性。如果两个或多个事物中发生了变化，但不会影响其他事物，则它们是正交的。当系统的各组建相互高度依赖时，就不再具有局部修正

> Eliminate Effects between Unrelated Things
> 消除无关事物之间的影响

**团队内部的正交**

如果团队的组织有许多重叠，各个成员就会对责任该到困惑，或因责任共享而懈怠。不仅如此，每次的需求变动都需整个团队开一次会，因为他们中的任何人都可能收到影响。

把团队由责任划分为不同的小组。可以从基础设施和应用分离着手。如果应用功能的划分显而易见，那就可以依次分组，尽量将人员之间的责任正交。**但不同组员之间的交流必不可少**

**设计与系统的正交**

系统应该由一组相互协作的模块组成，每个模块都实现不依赖于其他模块的功能。有时，这些组件被组织为多个层次，每层提供一级抽象

对于正交设计，有一种简单的测试方法：问自己，如果显著的改变某个特定功能背后的需求，有多少模块会受到影响？（在严格的正交系统中应该只有一个）

**不要依赖你无法控制的事物**

**通过构建单元测试来监测模块正交性**

#### 可撤销性

始终要考虑撤销决策的情况。因为没有决策会是最终决策，情况总是在变。