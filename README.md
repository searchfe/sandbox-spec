# sandbox-spec

> 本文用于描述运行于浏览器Web环境的Window&Document沙盒环境Javascript代码API规范。适用于自行封装的闭包运行环境、浏览器Web worker以及组件运行环境等需要直接和浏览器原生API交互的代码。

## 约定

关于API的描述，格式如下：

### 描述语言规范

API相关描述，遵循以下关键字描述规范：

    must
    must not
    required
    should
    should not
    recommended
    may
    optional

### API描述格式

使用三级标题定义API类别，例如：``### Dom``

使用四级标题定义API具体描述，例如：

#### API Name

Write API description here.

*API参数是API描述中必须说明的部分，说明时使用表格进行参数的描述*

API Params Table

| Name | Type | Description |
| First Params | string | 第一个参数 |

