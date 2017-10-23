# sandbox-spec

本文用于描述运行于浏览器 Web 环境的 Window/Document 沙盒环境的 API 规范。
适用于自行封装的闭包运行环境、浏览器 Web Worker 以及其他组件化的运行环境等，
需要与浏览器原生 API 进行隔离的代码。

> 本文档中对于 "必须（must）", "不得（must not）", "应该（should）", "不应（should not）", "推荐（recommended）", "可以（may）", "可选（optional）" 的使用，遵循 [RFC 2119][rfc2119]。

## API 设计原则

**1. 与原生API尽量保持一致**

函数名、参数、返回值的类型、名字与原生 API 保持一致，执行方式（例如同步/异步，是否抛出异常）也应保持一致。

**2. 原生没有的API，可进行拓展**

如果没有可用的原生 API，可以设计一个 API 并完成文档并发送 PR 以供 Review。

## API 文档格式约定

* 每个文件描述一个对象/类。
* 文件名与类名保持一致，例如 `HTMLElement.md`。
* 所有对其他类的引用都给出文档链接，可以引用 MDN 文档。

在 [/spec/demo](https://github.com/searchfe/sandbox-spec/blob/master/spec/demo.md)

## API 文档内容约定

* 每个对象的 API 分为属性、方法和事件，鼓励文档之间互相引用。
* 每个属性应说明类型，只读状态（如果有的话）。
* 每个方法应说明参数与返回值，分别说明类型、可选性和默认值。
* 每个事件应给出触发时机，以及事件对象的文档链接。

## 常见问题

* 同步 API 不得直接改为异步调用设计，因为这违背了设计原则1。

[rfc2119]: https://tools.ietf.org/html/rfc2119
