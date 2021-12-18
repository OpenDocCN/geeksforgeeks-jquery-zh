# jQWidgets jqxRangeSelector 快照属性

> 原文:[https://www . geeksforgeeks . org/jqwidgets-jqxrangeselector-snaptoticks-property/](https://www.geeksforgeeks.org/jqwidgets-jqxrangeselector-snaptoticks-property/)

jQWidgets 是一个 JavaScript 框架，用于为 PC 和移动设备制作基于 web 的应用程序。它是一个非常强大、优化、独立于平台并且得到广泛支持的框架。jqxRangeSelector 小部件用于表示 jQuery 范围滑块，该滑块可轻松用于选择数值或日期范围值。这个小部件用于设置数字、天、周、月、年等范围。

snapToTicks 属性用于设置或返回滑块是否会与主要刻度和次要刻度对齐。它接受布尔类型值，默认值为真。

**语法:**

设置快照打包属性。

```
$('selector').jqxRangeSelector({ 
    snapToTicks: Boolean 
});
```

返回快照打包属性。

```
var snapToTicks = $('selector')
    .jqxRangeSelector('snapToTicks');
```

**链接文件:**从给定的链接 https://www.jqwidgets.com/download/.下载 jQWidgets 在 HTML 文件中，找到下载文件夹中的脚本文件。

> <link rel="”stylesheet”" href="”jqwidgets/styles/jqx.base.css”" type="”text/css”">
> <脚本类型= " text/JavaScript " src = " scripts/jquery-1 . 11 . 1 . min . js "></脚本类型>
> <脚本类型= " text/JavaScript " src = " jqwidgets/jqxcore . js "></脚本类型>
> <脚本类型= " text/JavaScript " src = " jqwidgets/jqx-all . js

下面的例子说明了 jQWidgets jqxRangeSelector Snaptotics 属性。

**示例:**

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
        src="jqwidgets/jqxcore.js"></script>
    <script type="text/javascript" 
        src="jqwidgets/jqx-all.js"></script>
    <script type="text/javascript" 
        src="jqwidgets/jqxdata.js"></script>
    <script type="text/javascript" 
        src="jqwidgets/jqxrangeselector.js"></script>

    <style>
        h1,
        h3 {
            text-align: center;
        }

        #jqxRS {
            width: 100%;
            margin: 0 auto;
        }
    </style>
</head>

<body>
    <h1 style="color: green;">
        GeeksforGeeks
    </h1>

    <h3>
        jQWidgets jqxRangeSelector snapToTicks Property
    </h3>

    <div id="jqxRS"></div>

    <script type="text/javascript">
        $(document).ready(function() {
            $("#jqxRS").jqxRangeSelector({
                width: 400,
                height: 20,
                min: 0,
                max: 100,
                range: {
                    from: 10,
                    to: 80
                },
                snapToTicks: true
            });
        });
    </script>
</body>

</html>
```

**输出:**

![](img/55f13a7194fe01ef00691b8213cbc742.png)

**参考:**[https://www . jqwidgets . com/jquery-widgets-documentation/documentation/jqxrange selector/jquery-range selector-API . htm](https://www.jqwidgets.com/jquery-widgets-documentation/documentation/jqxrangeselector/jquery-rangeselector-api.htm)