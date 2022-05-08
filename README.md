<!--
 * @Author       : Cherry
 * @Date         : 2022-05-08 19:39:09
 * @LastEditors  : Cherry
 * @LastEditTime : 2022-05-08 20:39:26
 * @Description  : 通过手写jquery代码理解设计风格
-->

# 声明

非本人源码。
源码链接：https://github.com/FrankFang/dom-2-prototype/blob/master/src/jquery.js

# jQuery 中的设计模式

1. jQuery 是非典型构造函数，它没有使用 new 构造函数，并且它的 j 是小写
2. 它的链式风格支持多种参数调用，这个模式叫做重载
3. 用闭包隐藏细节，给定一个参数，并且让用户只能通过这个参数来操作函数
4. $div.text()可读也可写，getter/ setter
5. $.fn 是 $.prototype 的别名
6. jQuery 针对不同浏览器使用不同代码，适配器

# jQuery 的实现

我认为，尽管 jQuery 已经过时，但是仍然有必要自己手写 jQuery，通过写 jQuery 来理解 jQuery 是怎么被构造出来的。
在学 CSS 的时候，方老师就说，你只需要记住就是这样写的，不要问为什么。但是 JS 是不同的，只有顺序执行语句、if...else...语句和 for 循环。但是我仍然需要询问，这是为什么？
这就是代码的简洁之美啊，从 jQuery 中我窥见了一角。
