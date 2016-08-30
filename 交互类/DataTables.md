交互类
===

## DataTables

> 综合表格插件，基于jQuery开发，应用灵活，可以配合DataTables Editor形成完成的表格编辑工具。

![](../images/datatables.png)

**Official：** 
- https://datatables.net/
- https://editor.datatables.net/ （Editor）

**Features：**
- 支持分页、即时搜索、多行排序
- 支持多种形式数据源：**DOM元素**、**Javascript对象**、**ajax**、**json**，丰富的数据源选项
- 样式定制，自带样式或使用jQuery UI、Bootstrap等，可自定义
- 支持多种第三方扩展组件，自定义控件
- 可扩展的options，清晰的API
- 自定义行列功能性操作
- 快速的过滤选项开发

**Git:**
- https://github.com/DataTables/DataTables

**DEMO:**
- https://datatables.net/examples/index
- https://editor.datatables.net/examples/index

**Doc：**
- https://datatables.net/reference/index
- https://editor.datatables.net/reference/index

**Example：**
```html
<table id="example" class="display" cellspacing="0" width="100%">
        <thead>
            <tr>
                <th>First name</th>
                <th>Last name</th>
                <th>Position</th>
                <th>Office</th>
                <th>Salary</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Tiger</td>
                <td>Nixon</td>
                <td>System Architect</td>
                <td>Edinburgh</td>
                <td>$320,800</td>
            </tr>
            <tr>
                <td>Garrett</td>
                <td>Winters</td>
                <td>Accountant</td>
                <td>Tokyo</td>
                <td>$170,750</td>
            </tr>
            <tr>
                <td>Ashton</td>
                <td>Cox</td>
                <td>Junior Technical Author</td>
                <td>San Francisco</td>
                <td>$86,000</td>
            </tr>
        </tbody>
    </table>
```

```javascript
$('#example').DataTable( {
	scrollY: 300,
    paging:   false,
    ordering: false,
    info:     false
} );
```
show message!

## 