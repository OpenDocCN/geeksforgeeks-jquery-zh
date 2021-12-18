# jqwidgets jqxlistox getselecteditem()方法

> [https://www.geeksforgeeks.org/jqwidgets-jqxlistbox-getselecteditem-method/](https://www.geeksforgeeks.org/jqwidgets-jqxlistbox-getselecteditem-method/)

**jQWidgets** 是一个 JavaScript 框架，用于为 PC 和移动设备制作基于 web 的应用程序。它是一个非常强大、优化、独立于平台并且得到广泛支持的框架。jqxListBox 用于说明一个 jQuery ListBox 小部件，它包含一个可选择元素的列表。

**getSelectedItem()** 方法用于从所述列表中返回所选项目。此外，返回值为对象类型，否则*为空*，以防未选择任何选定项目。它没有参数，并且返回一个对象。

返回值是具有以下字段的对象:

*   标签
*   价值
*   有缺陷的
*   检查
*   hasThreeStates
*   超文本标记语言
*   指数
*   组

**语法:**

```
var item = $("#jqxListBox").jqxListBox('getSelectedItem');  
```

**链接文件:**从链接下载 [jQWidgets](https://www.jqwidgets.com/download/) 。在 HTML 文件中，找到下载文件夹中的脚本文件。

> <link rel="”stylesheet”" href="”jqwidgets/styles/jqx.base.css”" type="”text/css”">
> <脚本类型=【text/JavaScript】src =【scripts/jquery-1 . 11 . 1 . min . js】></脚本>
> <脚本类型=【text/JavaScript】src =【jqwidgets/jqx-all . js】></脚本>
> <脚本类型=【text/JavaScript】src =【jqwidgets/jqxcore

**示例:**下面的示例说明了 jQWidgets 中的 jqxListBox**getSelectedItem()**方法。

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
            src=".jqwidgets/jqxbuttons.js"></script>
        <script type="text/javascript" 
            src="jqwidgets/jqxscrollbar.js"></script>
        <script type="text/javascript" 
            src="jqwidgets/jqxlistbox.js"></script>
    </head>

    <body>
        <center>
            <h1 style="color: green;">
                GeeksforGeeks
            </h1>

            <h3>
                jQWidgets jqxListBox getSelectedItem() Method
            </h3>

            <div id="jqxLB"></div>
            <br />
            <input type="button" id="jqxBtn" 
                style="padding: 5px 20px;" 
                value="get the selected item" />
        </center>

        <script type="text/javascript">
            $(document).ready(function () {
                var data = [
                  "Computer Science", 
                  "C Programming",
                  "C++ Programming"];

                $("#jqxLB").jqxListBox({
                    source: data,
                    width: "200px",
                    height: "80px",
                    selectedIndex: 2
                });

                $("#jqxBtn").on("click", function () {
                     var itm = $("#jqxLB").jqxListBox('getSelectedItem');
                     console.log("Selected item is: " + itm.label);
                });
            });
        </script>
    </body>
</html>
```

**输出:**

![](img/3e87d96ec2ee075940e4e5bdfa0e2210.png)

getSelectedItem 方法

**参考:**[https://www . jqwidgets . com/jquery-widgets-documentation/documentation/jqxlistbox/jquery-listbox-API . htm？搜索=](https://www.jqwidgets.com/jquery-widgets-documentation/documentation/jqxlistbox/jquery-listbox-api.htm?search=)