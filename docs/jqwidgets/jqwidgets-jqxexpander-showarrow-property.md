# jQWidgets jqxExpander show arrow 属性

> 原文:[https://www . geesforgeks . org/jqwidgets-jqxexpander-show arrow-property/](https://www.geeksforgeeks.org/jqwidgets-jqxexpander-showarrow-property/)

**jQWidgets** 是一个 JavaScript 框架，用于为 PC 和移动设备制作基于 web 的应用程序。它是一个非常强大和优化的框架，独立于平台，并得到广泛支持。jqxExpander 代表一个 jQuery 小部件，显示标题和内容部分。单击标题部分展开或折叠内容。

***显示箭头*** **属性**用于设置或返回表头的箭头是否显示。接受布尔类型值，默认值为*真*。

**语法:**

设置*显示箭头*属性。

```
$('selector').jqxExpander({ showArrow: String });
```

返回*显示箭头*属性。

```
var showArrow = $('selector').jqxExpander('showArrow');
```

**链接文件:**从给定链接下载 [jQWidgets](https://www.jqwidgets.com/download/) 。在 HTML 文件中，找到下载文件夹中的脚本文件。

> <link rel="”stylesheet”" href="”jqwidgets/styles/jqx.base.css”" type="”text/css”">
> < link rel= "样式表" href = " jqwidgets/style/jqx . energy blue . CSS " type = " text/CSS "/>
> <脚本类型= " text/JavaScript " src = " scripts/jquery-1 . 11 . 1 . min . js "></脚本>
> <脚本类型= " text/JavaScript " src = " jqwidgets/jqx-all

**示例:**以下示例说明了 jQWidgets jqxExpander*showArrow*属性。

## 超文本标记语言

```
<!DOCTYPE html>
<html lang="en">

<head>
    <link rel="stylesheet" href=
        "jqwidgets/styles/jqx.base.css" type="text/css" />
    <script type="text/javascript" 
        src="scripts/jquery-1.11.1.min.js"></script>
    <script type="text/javascript" 
        src="jqwidgets/jqx-all.js"></script>
    <script type="text/javascript" 
        src="jqwidgets/jqxcore.js"></script>
    <script type="text/javascript" 
        src="jqwidgets/jqxexpander.js"></script>
</head>

<body>
    <center>
        <h1 style="color: green;">
            GeeksforGeeks
        </h1>

        <h3>
            jQWidgets jqxExpander showArrow Property
        </h3>

        <div id='jqxExp'>
            <div>GeeksforGeeks</div>

            <div style="text-align: justify;">
                A Computer Science portal for geeks. 
                It contains well written, well thought 
                and well explained computer science 
                and programming articles, ...
            </div>
        </div>
    </center>

    <script type="text/javascript">
        $(document).ready(function() {
            $("#jqxExp").jqxExpander({ 
                width: 250, 
                height: 150,
                showArrow: false
            });
        });
    </script>
</body>

</html>
```

**输出:**

![](img/6224d1e85d2c6d856397e0abc7840fe7.png)

**参考:**[https://www . jqwidgets . com/jquery-widgets-documentation/documentation/jqxexpander/jquery-expander-API . htm](https://www.jqwidgets.com/jquery-widgets-documentation/documentation/jqxexpander/jquery-expander-api.htm)