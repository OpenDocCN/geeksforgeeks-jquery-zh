# jQWidgets jqxTagCloud altextcase 属性

> 原文:[https://www . geeksforgeeks . org/jqwidgets-jqxtagcloud-altextcase-property/](https://www.geeksforgeeks.org/jqwidgets-jqxtagcloud-altertextcase-property/)

**jQWidgets** 是一个 JavaScript 框架，用于为 PC 和移动设备制作基于 web 的应用程序。它是一个非常强大、优化、独立于平台并且得到广泛支持的框架。****jqxTagCloud**用于显示一组与网站上的文章、帖子或视频相匹配的用户生成的标签。**

****altextcase****属性**用于设置或获取 altextcase 属性，该属性用于指定指定的 *jqxTagCloud* 的标签将被排序的字段。它的可能值是“无”、“全低”、“全高”、“第一高”、“标题大小写”。**

****语法:****

*   **设置*替代文本案例*属性:**

    ```
    $('#jqxTagCloud').jqxTagCloud({ alterTextCase: 'allUpper' });
    ```

*   **要获取*altextcase*属性:**

    ```
    var value = $('#jqxTagCloud').jqxTagCloud({ 'alterTextCase' });
    ```

****链接文件:**从给定链接下载 [jQWidgets](https://www.jqwidgets.com/download/) 。在 HTML 文件中，找到下载文件夹中的脚本文件。**

> <link rel="”stylesheet”" href="”jqwidgets/styles/jqx.base.css”" type="”text/css”"> **<脚本类型=“text/JavaScript”src =“scripts/jquery . js”></脚本>
> <脚本类型=“text/JavaScript”src =“jqwidgets/jqxcore . js”></脚本>
> <脚本类型=“text/JavaScript”src =“jqwidgets/jqxdata . js”><**

****示例:**以下示例说明了 jQWidgets jqxTagCloud**altextcase**T4 属性。在下面的例子中，alterTextCase 属性的值被设置为“allUpper”。**

## **超文本标记语言**

```
<!DOCTYPE html>
<html lang="en">

<head>
    <link rel="stylesheet"
          href="jqwidgets/styles/jqx.base.css" 
          type="text/css"/>
    <script type="text/javascript" 
            src="scripts/jquery.js">
    </script>
    <script type="text/javascript" 
            src="jqwidgets/jqxcore.js">
    </script>
    <script type="text/javascript" 
            src="jqwidgets/jqxdata.js">
    </script>
    <script type="text/javascript" 
            src="jqwidgets/jqxtagcloud.js">
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
            jQWidgets jqxTagCloud alterTextCase Property
        </h3>
        <div id="Tag_Cloud"></div>
        <input type="button" style="margin: 28px;" 
               id="button_for_alterTextCase"
                  value="Value of the alterTextCase property"/>
        <div id="log"></div>
        <script type="text/javascript">
            $(document).ready(function () {
                var Data_for_TagCloud = [
                    { Name: "GFG", Rating: 4 },
                    { Name: "is a", Rating: 3 },
                    { Name: "CS", Rating: 2 },
                    { Name: "Portal.", Rating: 5 },
                ];
                var dataAdapter = new
                    $.jqx.dataAdapter({
                        localData: Data_for_TagCloud
                    });
                $('#Tag_Cloud').jqxTagCloud({
                    width: 450,
                    source: dataAdapter,
                    displayMember: 'Name',
                    valueMember: 'Rating',
                    alterTextCase: 'allUpper'
                });
                $("#button_for_alterTextCase").
                    jqxButton({
                        width: 300
                    });
                $("#button_for_alterTextCase").jqxButton().
                    click(function () {
                        var a = $('#Tag_Cloud').jqxTagCloud(
                            'alterTextCase');
                        $("#log").html(a);
                    });
            });
        </script>
    </center>
</body>

</html>
```

****输出:****

**![](img/397963a6bc9a59227511cb2decac0864.png)**

****参考:**[https://www . jqwidgets . com/jquery-widgets-documentation/documentation/jqxtagcloud/jquery-tag cloud-API . htm](https://www.jqwidgets.com/jquery-widgets-documentation/documentation/jqxtagcloud/jquery-tagcloud-api.htm)**