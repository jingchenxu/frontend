## sugar

> 在原生对象上增加一些工具方法

![](../images/sugar.png)

**Official：** 
- https://sugarjs.com/

**Features：**
- 在原生对象上进行扩展，可能与未来浏览器产生一定的不兼容

**Git:**
- https://github.com/andrewplummer/Sugar/

**Demo:**
- https://sugarjs.com/docs/

**Doc：**
- https://sugarjs.com/docs/

**Example：**
```html

```

```javascript
Sugar.Array.construct(4, function(i) {
  return i * i;
});
[0, 1, 4, 9]
