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
3. 用闭包隐藏细节，给定一个参数，并且让用户只能通过这个参数来操作函数，避免全局污染
4. $div.text()可读也可写，getter/ setter
5. $.fn 是 $.prototype 的别名
6. jQuery 针对不同浏览器使用不同代码，适配器

# jQuery 的实现
我怎么想不到！

