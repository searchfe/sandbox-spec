# HTMLElement

> 这是一个 Demo 文档，不可认真。

`HTMLElement` 是用来干嘛的、现在是否推荐使用、有什么类似的 API 没有可以参照。
大概工作原理是怎样的，麻烦的话可以写几段话，来个描述图。

## 属性

*继承* 自 `Element` 的所有属性。

* `.innerHTML`：类型为 `String`。用来设置和获取元素内的 HTML。
* `.outerHTML`：类型为 `String`，只读。用来获取元素的 HTML。

## 方法

*继承* 自 `Element` 的所有方法。

**.querySelector(selector, context)**

获取第一个符合 `selector` 的后代元素节点，按照树序排序。

* `selector`：类型为 `String`，没有默认值。一个用来选中元素的 CSS 选择符。
* `context`：类型为 [Element][eg]，默认值为当前 `HTMLElement`。选取节点的上下文。
* 返回值：类型为 `Array`，每一项是一个 `Element`。

**.querySelectorAll(selector, context)**

获取所有符合 `selector` 的后代元素节点。

* `selector`：类型为 `String`，没有默认值。一个用来选中元素的 CSS 选择符。
* `context`：类型为 [Element][eg]，默认值为当前 `HTMLElement`。选取节点的上下文。
* 返回值：类型为 `Array`，每一项是一个 `Element`。

## 事件

*继承* 自 `Element` 的所有事件，除了 `explode` 之外。

* `click`：类型为 [ClickEvent][eg]。点击事件，在鼠标点击时发生。
* `blur`：类型为 [BlurEvent][eg]。焦点离开事件，在输入焦点离开控件时发生。

[eg]: http://example.com
