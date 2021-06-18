# JSBridge

> JSBridge 用于 Hybrid 混合开发，WebView(原生容器)通过 **解释器** 调用 **全局window.JavaScript 对象** 或 **JavaScript 字符串**执行JS脚本，相对的JS通过**WebView拦截URL Schema** 或WebView**注入原生API到JS-Context** 调用原生的API。

- URL拦截

  URL Schema 是一种特殊的 URL，支持自定义，基本格式为：

  > `<protocol>://<host>/<path>[#hash][?qeury]`

  因此，在更改了地址后，WebView可以拦截地址，并根据URL解析操作及参数

- 原生 API Context 注入

  原生API通过将Context对象，注入到全局 window 对象中(如：window.JSBridge)，即可以在JS环境中调用API


### 参考

- [深入浅出JSBridge](https://juejin.cn/post/6936814903021797389)
- [JS Bridge 通信原理与实践](https://juejin.cn/post/6916316666208976904)
