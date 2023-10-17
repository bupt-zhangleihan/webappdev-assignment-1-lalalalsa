# 用 DOM 干更多事

## 说明

选取一个 DOM 元素，并通过它对 DOM 进行更深入的研究。访问 MDN 的 [DOM 接口的清单](https://developer.mozilla.org/docs/Web/API/Document_Object_Model) 并挑选一个。在网络上寻找一个使用了这个元素的网页，并解释如何使用它。

## 回答

`MutationObserver`：

`MutationObserver` 接口在 DOM API 中提供了监视 DOM 树更改的能力，例如属性修改、子节点的添加或删除。以下是其使用的简化示例：

1. 使用回调创建一个 `MutationObserver` 实例来处理 DOM 变异。
2. 通过 `observe()` 方法配置观察器，指定目标节点和要监视的变异类型。
3. 在完成观察时，可选择使用 `disconnect()` 方法断开观察器。

`MutationObserver` 的实际示例可以在[这里](https://codepen.io/milofultz/pen/LYjPXPw)看到。在这个网站中可以实现响应 DOM 的实时变化，可以帮助用户更方便的进行动态网页的编写。
