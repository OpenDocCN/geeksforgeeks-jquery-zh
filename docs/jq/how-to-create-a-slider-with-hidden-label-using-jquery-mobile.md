# 如何使用 jQuery Mobile 创建隐藏标签的滑块？

> 原文:[https://www . geeksforgeeks . org/如何使用 jquery-mobile/](https://www.geeksforgeeks.org/how-to-create-a-slider-with-hidden-label-using-jquery-mobile/) 创建带有隐藏标签的滑块

jQuery Mobile 是一种基于网络的技术，用于制作可在所有智能手机、平板电脑和台式机上访问的响应内容。在本文中，我们将使用 jQuery Mobile 创建一个带有隐藏标签的滑块。

**方法:**添加项目所需的 jQuery Mobile 脚本。

> <link rel="”stylesheet”" href="”http://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.css”">
> <脚本 src = " http://code . jquery . com/jquery-1 . 11 . 1 . min . js "></脚本>
> <脚本 src = " http://code . jquery . com/mobile/1 . 4 . 5/jquery . mobile-1 . 4 . 5 . min . js "></脚本>

**示例:**我们将使用 jQuery Mobile 创建一个基本滑块。滑块是一种使用滑块插入数据的输入类型。我们使用 type="range "属性和<输入>元素来创建一个滑块。

## 超文本标记语言

```
<!DOCTYPE html>
<html>

<head>
    <link rel="stylesheet" href=
"http://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.css" />

    <script src=
        "http://code.jquery.com/jquery-1.11.1.min.js">
    </script>

    <script src=
"http://code.jquery.com/mobile/1.4.5/jquery.mobile-1.4.5.min.js">
    </script>
</head>

<body>
    <center>
        <h1>GeeksforGeeks</h1>

        <h4>
            Design a Slider with hidden 
            Label using jQuery Mobile
        </h4>

        <form style="width: 50%;">
            <label for="slider" 
                class="ui-hidden-accessible">
                Slider with hidden Label:
            </label>

            <input type="range" name="slider" 
                id="slider" data-track-theme="b" 
                data-theme="b" min="0" max="100"
                value="50">
        </form>
    </center>
</body>

</html>
```

**输出:**

![](img/44bfb1a21aa5ea7e8647289259225676.png)