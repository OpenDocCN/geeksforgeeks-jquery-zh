# jQWidgets jqxRating 项目高度属性

> 原文:[https://www . geesforgeks . org/jqwidgets-jqxrating-item height-property/](https://www.geeksforgeeks.org/jqwidgets-jqxrating-itemheight-property/)

**jQWidgets** 是一个 JavaScript 框架，用于为 PC 和移动设备制作基于 web 的应用程序。它是一个非常强大、优化、独立于平台并且得到广泛支持的框架。jqxRating 代表一个 jQuery 小部件，显示*评级*选项来选择评级。此小部件用于配置 jqxRating 小部件项目的大小、图像和显示项目的数量等。

*项目高度*属性用于设置或返回评级项目的高度。它接受数字类型值，默认值为*自动*。

**语法:**

设置*项目高度*属性。

```
$('selector').jqxRating({ itemHeight: Number });
```

返回*物品高度*属性。

```
var itemHeight = $('selector').jqxRating('itemHeight');
```

**链接文件:**从给定链接下载 [jQWidgets](https://www.jqwidgets.com/download/) 。在 HTML 文件中，找到下载文件夹中的脚本文件。

> <link rel="”stylesheet”" href="”jqwidgets/styles/jqx.base.css”" type="”text/css”">
> < link rel= "样式表" href = " jqwidgets/style/jqx . energy blue . CSS " type = " text/CSS "/>
> <脚本类型= " text/JavaScript " src = " scripts/jquery-1 . 11 . 1 . min . js "></脚本>
> <脚本类型= " text/JavaScript " src = " jqwidgets/jqx-all

**示例:**以下示例说明了 jQWidgets jqxRating*item height*属性。

## 超文本标记语言

```
<!DOCTYPE html>
<html lang="en">

<head>
    <link rel="stylesheet" href=
        "jqwidgets/styles/jqx.base.css" type="text/css" />
    <link rel="stylesheet" href=
        "jqwidgets/styles/jqx.energyblue.css" type="text/css" />
    <script type="text/javascript" 
        src="scripts/jquery-1.11.1.min.js"></script>
    <script type="text/javascript" 
        src="jqwidgets/jqx-all.js"></script>
    <script type="text/javascript" 
        src="jqwidgets/jqxcore.js"></script>
    <script type="text/javascript" 
        src="jqwidgets/jqxrating.js"></script>
</head>

<body>
    <center>
        <h1 style="color: green;">
            GeeksforGeeks
        </h1>

        <h3>
            jQWidgets jqxRating itemHeight Property
        </h3>

        <div id='jqxRating'></div>
    </center>

    <script type="text/javascript">
        $(document).ready(function() {
            $("#jqxRating").jqxRating({
                width: 200,
                itemHeight: 40,
                count: 10
            });
        });
    </script>
</body>

</html>
```

**输出:**

![](img/9515d1179693edd90f6120a16ef8616e.png)

**参考:**[https://www . jqwidgets . com/jquery-widgets-documentation/documentation/jqxrating/jquery-rating-入门. htm](https://www.jqwidgets.com/jquery-widgets-documentation/documentation/jqxrating/jquery-rating-getting-started.htm)