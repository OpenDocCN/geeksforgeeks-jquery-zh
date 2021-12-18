# jQWidgets jqxPopover 标题属性

> 原文:[https://www . geesforgeks . org/jqwidgets-jqxpopover-title-property/](https://www.geeksforgeeks.org/jqwidgets-jqxpopover-title-property/)

**jQWidgets** 是一个 JavaScript 框架，用于为 PC 和移动设备制作基于 web 的应用程序。它是一个非常强大、优化、独立于平台并且得到广泛支持的框架。 **jqxPopover** 是内容的小覆盖，用于在用户点击时显示任何元素的次要信息。

**标题**属性用于设置或获取指定 jqxPopover 小部件的标题。

**语法:**

*   要设置标题属性:

    ```
    $('#jqxPopover').jqxPopover({title: String});
    ```

*   要获取标题属性:

    ```
    var arrowOffsetValue = $('#jqxPopover').jqxPopover('title');
    ```

**链接文件:**从给定链接下载 https://www.jqwidgets.com/download/。在 HTML 文件中，找到下载文件夹中的脚本文件。

> <link rel="”stylesheet”" href="”jqwidgets/styles/jqx.base.css”" type="”text/css”/">
> <脚本类型=“text/JavaScript”src =“scripts/jquery . js”></script>
> <脚本类型=“text/JavaScript”src =“jqwidgets/jqxcore . js”></script>
> <脚本类型=“text/JavaScript”src =“jqwidgets/jqxbuttons . js”><

**示例:**下面的示例说明了 jQWidgets jqxPopover**title***T5*属性。在下面的例子中，**标题**属性的值被设置为“公司名称”。

## 超文本标记语言

```
<!DOCTYPE html>
<html lang="en">

<head>
    <link rel="stylesheet" 
          href="jqwidgets/styles/jqx.base.css"
          type="text/css" />
    <script type="text/javascript" 
               src="scripts/jquery.js">
    </script>
    <script type="text/javascript" 
               src="jqwidgets/jqxcore.js">
    </script>
    <script type="text/javascript" 
               src="jqwidgets/jqxbuttons.js">
    </script>
    <script type="text/javascript" 
               src="jqwidgets/jqxpopover.js">
    </script>
    <script type="text/javascript" 
               src="jqwidgets/jqx-all.js">
    </script>
</head>

<body>
    <center>
        <h1 style="color:green;">
            GeeksforGeeks
        </h1>
        <h3>
            jQWidgets jqxPopover title Property
        </h3>
        <div id='jqx_Popover'>
            <center>
                GeeksforGeeks
            </center>
        </div>

        <input type="button" style="margin: 28px;" 
               id="button_for_Popover" 
               value="Toggle the Popover" />
        </br>
        <input type="button" style="margin: 65px;" 
               id="button_for_title" 
               value="Value of the title property" />

        <div id="log"></div>
        <script type="text/javascript">
            $(document).ready(function () {
                $("#jqx_Popover").jqxPopover({
                    width: 180,
                    height: 80,
                    theme: 'energyblue',
                    autoClose: false,
                    selector: $("#button_for_Popover"),
                    title: 'Company_Name'
                });
                $("#button_for_Popover").jqxButton({
                    width: 200,
                    theme: 'energyblue'
                });
                $("#button_for_title").jqxButton({
                    width: 300,
                    theme: 'energyblue'
                });
                $('#button_for_title').jqxButton().
                    click(function () {
                        var Value_of_title =
                            $('#jqx_Popover').jqxPopover(
                                'title');
                        $("#log").html((Value_of_title));
                    })
            });
        </script>
    </center>
</body>

</html>
```

**输出:**

![](img/040f3f8930e955121e906123ce5b5caf.png)

**参考:**[https://www . jqwidgets . com/jquery-widgets-documentation/documentation/jqxpopover/jquery-popover-API . htm？搜索=](https://www.jqwidgets.com/jquery-widgets-documentation/documentation/jqxpopover/jquery-popover-api.htm?search=)