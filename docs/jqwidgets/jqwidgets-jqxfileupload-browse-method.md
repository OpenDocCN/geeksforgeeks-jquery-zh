# jQWidgets jqxFileUpload 浏览()方法

> 原文:[https://www . geesforgeks . org/jqwidgets-jqxfileupload-browse-method/](https://www.geeksforgeeks.org/jqwidgets-jqxfileupload-browse-method/)

**jQWidgets** 是一个 JavaScript 框架，用于为 PC 和移动设备制作基于 web 的应用程序。它是一个非常强大和优化的框架，独立于平台，并得到广泛支持。 **jqxFileUpload** 是一个小部件，可以用来选择文件并上传到服务器。它还支持自动上传和多文件上传。

**browse()** 方法用于设置按钮，该按钮显式地使用另一个按钮来 b 文件的行。不取任何参数，不返回值。

**语法:**

```
$('#jqxFileUpload').jqxFileUpload('browse');
```

**链接文件:**从链接下载 [jQWidgets](https://www.jqwidgets.com/download/) 。在 HTML 文件中，找到下载文件夹中的脚本文件。

> <link type="”text/css”" rel="”Stylesheet”" href="”jqwidgets/styles/jqx.base.css”">
> <脚本类型=【文本/JavaScript】src =【脚本/jquery-1 . 11 . 1 . min . js】></脚本>
> <脚本类型=【文本/JavaScript】src =【jqwidgets/jqxcore . js】></脚本>
> <脚本类型=【文本/JavaScript】src =【jqwidgets/jqxbuttons . js

**示例:**下面的示例说明了 jQWidgets 中的 jqxFileUpload **browse()** 方法。

## 超文本标记语言

```
<!DOCTYPE html>
<html lang="en">

<head>
    <link type="text/css" rel="Stylesheet" 
          href="jqwidgets/styles/jqx.base.css" />
    <script type="text/javascript" 
              src="scripts/jquery-1.11.1.min.js">
    </script>
    <script type="text/javascript" 
              src="jqwidgets/jqxcore.js">
    </script>
    <script type="text/javascript" 
            src="jqwidgets/jqxbuttons.js">
    </script>
    <script type="text/javascript" 
            src="jqwidgets/jqxfileupload.js">
    </script>

</head>

<body>
    <h1 style="color: green">
          GeeksforGeeks 
      </h1>
    <h3>jQWidgets jqxFileUpload browse() method</h3>  
    <div id="gfg"></div>
    <input style="margin-top: 20px;" type="button" 
           id="jqxButton" value="Browse for a file" />

    <script type="text/javascript">
          $(document).ready(function () {
              $('#gfg').jqxFileUpload({ 
                  theme: 'energyblue',
                  width: 300,
                  uploadUrl: 'upload.php',
              });
              $('#jqxButton').on('click', function () {
                  $('#gfg').jqxFileUpload('browse');
              });
          });
    </script>
</body>

</html>
```

**输出:**

![](img/f01546036963b5e9e133f5c5e517c269.png)

**参考:**[https://www . jqwidgets . com/jquery-widgets-documentation/documentation/jqxfileupload/jquery-file-upload-API . htm](https://www.jqwidgets.com/jquery-widgets-documentation/documentation/jqxfileupload/jquery-file-upload-api.htm)