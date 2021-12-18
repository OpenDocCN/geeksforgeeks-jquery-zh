# jquery ui date picker monthname option

> 哎哎哎:# t0]https://www . geeksforgeeks . org/jquery-ui-date picker-monthname 选项/

jQuery UI 由 GUI 小部件、视觉效果和使用 jQuery、CSS 和 HTML 实现的主题组成。jQuery 用户界面非常适合为网页构建用户界面。 jQueryUI 中的 jQueryUI Datepickers 小部件允许用户轻松直观地输入日期。在本文中，我们将看到如何在 jQuery UI Datepicker 中使用 **monthNames 选项** 。 **月名称选项** 用于在 jQuery UI 日期选择器中设置月份名称。

**语法:**

```
$(".selector").datepicker(
   {monthNames: [ "January", "February", "March", 
   "April", "May", "June", "July", "August", 
   "September", "October", "November", "December" ]}
);
```

**方法:**首先，添加项目所需的 jQuery UI 脚本。

> <link href="“https://code.jquery.com/ui/1.10.4/themes/ui-lightness/jquery-ui.css”" rel="“stylesheet”">
> <脚本 src = " https://code . jquery . com/jquery-1 . 10 . 2 . js "></脚本>
> <脚本 src = " https://code . jquery . com/ui/1 . 10 . 4/jquery-ui . js "></脚本>

**例 1:**

## 超文本标记语言

```
<!doctype html>
<html lang="en">

<head>
    <meta charset="utf-8">
    <link href=
"https://code.jquery.com/ui/1.10.4/themes/ui-lightness/jquery-ui.css"
        rel="stylesheet">

    <script src=
        "https://code.jquery.com/jquery-1.10.2.js">
    </script>

    <script src=
        "https://code.jquery.com/ui/1.10.4/jquery-ui.js">
    </script>

    <!-- JavaScript code -->
    <script>
        $(function () {
            $("#gfg").datepicker(
                {
                    dateFormat: "yy/dd/mm/MM",
                    monthNames: ["jan", "feb", "mar", 
                    "april", "may", "jun", "jul", 
                    "aug", "sep", "oct", "nov", "dec"]
                }
            );
        });
    </script>
</head>

<body>
    <h1>GeeksforGeeks</h1>
    <h3>jQuery UI | datepicker monthNames option</h3>

    <p>Enter Date: <input type="text" id="gfg"></p>
</body>

</html>
```

**输出:**

![](img/3033e4aa4ec86ae48200613113fb2de8.png)

**参考:**T2】https://api.jqueryui.com/category/widgets/