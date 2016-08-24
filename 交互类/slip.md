## Slip

> 通过滑动和拖动手势操作列表的UI库

![](../images/slip.gif)

**Official：** 
- https://kornel.ski/slip/

**Features：**
- 轻量
- 操作简单方便

**Git:**
- https://github.com/pornel/slip

**DEMO:**
- https://kornel.ski/slip/

**Doc：**
- https://www.awesomes.cn/repo/pornel/slip

**Example：**
```html

```

```javascript
var list = document.querySelector('ul#slippylist');
new Slip(list);

list.addEventListener('slip:beforeswipe', function(e) {
    if (shouldNotSwipe(e.target)) {
        e.preventDefault(); // won't move sideways if prevented
    }
});

list.addEventListener('slip:swipe', function(e) {
    // e.target list item swiped
    if (thatWasSwipeToRemove) {
        // list will collapse over that element
        e.target.parentNode.removeChild(e.target);
    } else {
        e.preventDefault(); // will animate back to original position
    }
});

list.addEventListener('slip:beforereorder', function(e) {
    if (shouldNotReorder(e.target)) {
        // if prevented element won't move vertically
        e.preventDefault();
    }
});

list.addEventListener('slip:beforewait', function(e) {
    if (isScrollingKnob(e.target)) {
        // if prevented element will be dragged (instead of page scrolling)
        e.preventDefault();
    }
});

list.addEventListener('slip:reorder', function(e) {
    // e.target list item reordered.
    if (reorderedOK) {
        e.target.parentNode.insertBefore(e.target, e.detail.insertBefore);
    } else {
        // element will fly back to original position
        e.preventDefault();
    }
});
```

## 