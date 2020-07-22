---
title: markdown使用
date: 2020.7.22
tags: markdown | 语法
---

## `注释`

- 代码法

<div style='display: none'>哈哈我是注释，不会在浏览器中显示。</div>

- html注释

<!-- 哈哈我是注释，不会在浏览器中显示。-->

<!--
    哈哈我是多段注释，
    不会在浏览器中显示。
-->

- hack方法

[//]: # (哈哈我是最强注释，不会在浏览器中显示。)
[^_^]: # (哈哈我是最萌注释，不会在浏览器中显示。)
[//]: <> (哈哈我是注释，不会在浏览器中显示。)
[comment]: <> (哈哈我是注释，不会在浏览器中显示。)

**************************************************

## `链接`

- 测试锚点

    <a href="#1">第一段</a>

    <a href="#2">第二段</a>

    <a href="#3">第三段</a>

    <divtop><a name="divtop">测试锚点1</a></divtop>  

- 图片链接

    [![Markdown语法大全(超级版)](https://upload-images.jianshu.io/upload_images/1496626-851332d4c4ebc3d8.png?imageMogr2/auto-orient/strip|imageView2/2/format/webp)](https://www.jianshu.com/p/ebe52d2d468f)

- 文字链接

    [1] 行内式

    参考了<a href="https://www.jianshu.com/p/ebe52d2d468f">这篇文章</a>

    欢迎阅读 [择势勤](https://www.jianshu.com/u/16d77399d3a7 "择势勤")

    [2] 参考式
    
    我经常去的几个网站[Google][1]、[Leanote][2]。

    [1]:http://www.google.com 
    [2]:http://www.leanote.com

    [3] 注脚

    使用 Markdown[^1]可以效率的书写文档, 直接转换成 HTML[^2]

    [^1]:Markdown是一种纯文本标记语言

    [^2]:HyperTextMarkupLanguage超文本标记语言

    [4] 锚点（页内超链接）

    [跳转到测试锚点1](#divtop) 

    <a name="1">第一段</a>

        这里是第一段的内容
        
    <a name="2">第二段</a>

        这里是第一段的内容

    <a name="3">第三段</a>

        这里是第一段的内容

    [5] 自动链接

    <http://example.com>

    <address@example.com>

**************************************************

## `分级标题、任务列表`

- 分级标题

        # 一级标题
        ## 二级标题
        ### 三级标题
        #### 四级标题
        ##### 五级标题
        ###### 六级标题  <!--最多6级标题-->

- 任务列表

    - [] 任务一 未做任务 `- + 空格 + [ ]`
    - [x] 任务二 已做任务 `- + 空格 + [x]`

**************************************************

## `无序列表、有序列表、定义型列表`

- 无序列表

    使用 *，+，- 表示无序列表。

    * 无序列表项 一
    + 无序列表项 二
    - 无序列表项 三
    
- 有序列表

    有序列表则使用数字接着一个英文句点。

    1. 有序列表项 一
    2. 有序列表项 二
    3. 有序列表项 三

- 定义型列表

    定义型列表由名词和解释组成。一行写上定义，紧跟一行写上解释。解释的写法:紧跟一个缩进(Tab)

    Markdown
    :   轻量级文本标记语言（左侧有一个可见的冒号和四个不可见的空格）

**************************************************

## `缩进、换行、空行、 对齐方式`

- 首行缩进

    【1】 &emsp;或&#8195; //全角<br>
    【2】 &ensp;或&#8194; //半角<br>
    【3】 &nbsp;或&#160;  //半角之半角
    
- 换行
        
        由于markdown编辑器的不同,可能在一行字后面，直接换行回车，也能实现换行，但是在Visual Studio Code上，想要换行必须得在一行字后面空两个格子才行。

- 空行

        在编辑的时候有多少个空行(只要这一行只有回车或者space没有其他的字符就算空行)，在渲染之后，只隔着一行。

- 对齐方式

    <center>行中心对齐</center>
    <p align="left">行左对齐</p>
    <p align="right">行右对齐</p>

**************************************************
        
## `斜体、粗体、删除线、下划线、背景高亮`

*斜体*或_斜体_<br>

**粗体**<br>

***加粗斜体***<br>

~~删除线~~<br>

++下划线++<br>

==背景高亮==

**************************************************

## `表格`

- 表格1

    -左对齐， :-: 中心对齐，-: 右对齐

    |学号|姓名|序号|
    |-|:-:|-:|
    |小明明|男|5|
    |小红|女|79|
    |小陆|男|192|

- 表格2

<!-- <center> -->
<table>
    <tr>
        <th rowspan="3">值班人员</th>
        <th>星期一</th>
        <th>星期二</th>
        <th>星期三</th>
        <th>星期三</th>
        <th>星期三</th>
    </tr>
    <tr>
        <td>李强</td>
        <td>张明</td>
        <td>王平</td>
        <td>王平</td>
        <td>王平</td>
    </tr>
    <tr>
        <td>李强</td>
        <td>张明</td>
        <td>王平</td>
        <td>王平</td>
        <td>王平</td>
    </tr>
</table>
<!-- </center> -->

**************************************************

## `插入图像`

<center>  <!--开始居中对齐-->

![GitHub set up](https://zh.mweb.im/asset/img/set-up-git.gif "图片Title")

</center> <!--结束居中对齐-->

**************************************************

## `多级引用`

>>> 请问 Markdwon 怎么用？ - 小白

>> 自己看教程！ - 愤青

> 教程在哪？ - 小白

**************************************************

## `LaTeX 公式`

$$\sum_{i=0}^n i^2 = \frac{(n^2+n)(2n+1)}{6}$$

质能守恒方程可以用一个很简洁的方程式 E = $m \times c^2$ 来表达。

详情请参考[Markdown数学公式语法](https://www.jianshu.com/p/e74eb43960a1) 和 [MathJax basic tutorial and quick reference](https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference)


**************************************************

## `字体`

<font face="黑体">我是黑体字</font>
<font face="微软雅黑">我是微软雅黑</font>
<font face="STCAIYUN">我是华文彩云</font>
<font color=#0099ff size=12 face="黑体">黑体</font>
<font color=gray size=5>gray</font>
<font color=#00ffff size=3>null</font>

**************************************************

## `代码块`

- 行内式

    C语言里的函数 `scanf()` 怎么使用？

- 缩进式多行代码

        #include <stdio.h>;
        int main(void)
        {
            printf("Hello world\n");
        }
    
- 用六个`包裹多行代码

    ```
    include <stdio.h>
    int main(void)
    {
        printf("Hello world\n");
    }
    ```
    
**************************************************

## `流程图`

```
graph LR
A-->B
```

```
sequenceDiagram
A->>B: How are you?
B->>A: Great!
```