## eventproxy

> javascript事件代理工具

![](../images/eventproxy.png)

**Official：** 
- http://underscorejs.org/

**Features：**
- 利用事件机制解耦复杂业务逻辑
- 移除被广为诟病的深度callback嵌套问题
- 将串行等待变成并行等待，提升多异步协作场景下的执行效率
- 友好的Error handling
- 无平台依赖，适合前后端，能用于浏览器和Node.js
- 兼容CMD，AMD以及CommonJS模块环境

**Git:**
- https://github.com/JacksonTian/eventproxy

**Demo:**
- https://github.com/JacksonTian/eventproxy

**Doc：**
- https://github.com/JacksonTian/eventproxy

**Example：**
```html

```

```javascript
var ep = EventProxy.create("template", "data", "l10n", function (template, data, l10n) {
  _.template(template, data, l10n);
});

$.get("template", function (template) {
  // something
  ep.emit("template", template);
});
$.get("data", function (data) {
  // something
  ep.emit("data", data);
});
$.get("l10n", function (l10n) {
  // something
  ep.emit("l10n", l10n);
});

```