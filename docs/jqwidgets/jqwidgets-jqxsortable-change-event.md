# jQWidgets jqxSortable 变更事件

> 原文:[https://www . geesforgeks . org/jqwidgets-jqxsortable-change-event/](https://www.geeksforgeeks.org/jqwidgets-jqxsortable-change-event/)

**jQWidgets** 是一个 JavaScript 框架，用于为 PC 和移动设备制作基于 web 的应用程序。它是一个非常强大、优化、独立于平台并且得到广泛支持的框架。 **jqxSortable** 代表一个 jQuery 插件，允许你使用鼠标对 HTML 列表或 *div* 标签中的元素重新排序。

当项目的 DOM 位置改变时，触发**改变**事件。

**语法:**

```
$('.jqxSortable').on('change', function (){
    // Code
});  
```

**链接文件:**从给定链接下载 [jQWidgets](https://www.jqwidgets.com/download/) 。在 HTML 文件中，找到下载文件夹中的脚本文件。

> <link type="”text/css”" rel="”Stylesheet”" href="”jqwidgets/styles/jqx.base.css”">
> <脚本类型= " text/JavaScript " src = " scripts/jquery-1 . 11 . 1 . min . js "></脚本类型>
> <脚本类型= " text/JavaScript " src = " jqwidgets/jqxcore . js "></脚本类型>
> <脚本类型= " text/JavaScript " src = " jqwidgets/globalize . js

**示例:**以下示例说明了 jQWidgets 中的 jqxSortable **变更**事件。

## 超文本标记语言

```
<!DOCTYPE html>
<html lang="en">

<head>
    <link type="text/css" rel="stylesheet" 
        href="jqwidgets/styles/jqx.base.css" />
    <script type="text/javascript" 
        src="scripts/jquery-1.11.1.min.js"></script>
    <script type="text/javascript" 
        src="jqwidgets/jqxcore.js"></script>
    <script type="text/javascript" 
        src="jqwidgets/globalization/globalize.js"></script>
    <script type="text/javascript" 
        src="jqwidgets/jqxsortable.js"></script>
</head>

<body>
    <h1 style="color: green">
        GeeksforGeeks 
    </h1>

    <h3>jQWidgets jqxSortable change event</h3>

    <div class="gfg">
        <div id="sort1">
            <div><li>C</li></div>
            <div><li>C++</li></div>
            <div><li>Python</li></div>
            <div><li>HTML</li></div>
            <div><li>CSS</li></div>
            <div><li>JavaScript</li></div>
        </div> 
    </div>

    <script type="text/javascript">
        $(document).ready(function () {
            $("#sort1").jqxSortable({
            });

            $('#sort1').on("change", function(){
                $('#sort1').append(`<br>`+'changed' );
            })
        });
    </script>
</body>

</html>
```

**输出:**

![](img/21f8317025e8ce93210ccab06637a3d2.png)

**参考:**[https://www . jqwidgets . com/jquery-widgets-documentation/documentation/jqxsortable/jquery-sortable-API . htm？搜索=](https://www.jqwidgets.com/jquery-widgets-documentation/documentation/jqxsortable/jquery-sortable-api.htm?search=)