---
title: markdown语法整理
copyright_author: Bruce Fc
copyright_author_href: 'https://brucefc.github.io/'
date: 2020-08-20 16:05:57
updated:
tags: markdown
categories: code
keywords: markdown md 整理
description:
top_img:
comments:
cover:
toc:
toc_number:
auto_open:
copyright:
copyright_url:
copyright_info:
mathjax:
katex:
aplayer:
highlight_shrink:
---

# MarkDown
## 简介
>Markdown 是一种轻量级标记语言，它允许人们使用易读易写的纯文本格式编写文档。
>Markdown 语言在 2004 由约翰·格鲁伯（英语：John Gruber）创建。
>Markdown 编写的文档可以导出 HTML 、Word、图像、PDF、Epub 等多种格式的文档。
>Markdown 编写的文档后缀为 `.md`, `.markdown`。

# MarkDown语法整理

## 标题

- 使用 `=` 和 `-` 标记一级和二级标题。
```
一级标题一级标题
===
二级标题二级标题
---
```

- 使用 `#` 号标记
```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

## 字体
- Markdown 可以使用以下几种字体：
```
*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___
```
展示如下：
    *斜体文本*
    _斜体文本_
    **粗体文本**
    __粗体文本__
    ***粗斜体文本***
    ___粗斜体文本___

## 分隔线
- 你可以在一行中用三个以上的星号`*`、减号`-`、底线`-`来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线：
```
***

* * *

*****

- - -

----------
```

## 删除线
- 如果段落上的文字要添加删除线，只需要在文字的两端加上两个波浪线 `~~` 即可
```
~~BAIDU.COM~~
```
展示如下：
    ~~BAIDU.COM~~

## 下划线
- 下划线可以通过 HTML 的 `<u>` 标签来实现：
```
<u>带下划线文本</u>
```
展示如下：
    <u>带下划线文本</u>

## 列表
- 无序列表
无序列表使用星号(`*`)、加号(`+`)或是减号(`-`)作为列表标记，这些标记后面要添加一个空格，然后再填写内容，例如：
```
* 第一项
* 第二项
* 第三项

+ 第一项
+ 第二项
+ 第三项


- 第一项
- 第二项
- 第三项
```
展示如下：
  * 第一项
  * 第二项
  * 第三项

  + 第一项
  + 第二项
  + 第三项

  - 第一项
  - 第二项
  - 第三项

- 有序列表
有序列表使用数字并加上 `.` 号来表示，如：
```
1. 第一项
2. 第二项
3. 第三项
```
展示如下：
  1. 第一项
  2. 第二项
  3. 第三项


## 引用
- 区块引用是在段落开头使用 `>` 符号 ，然后后面紧跟一个空格符号：
```
>这是区块引用例子
```
展示如下：
    >这是区块引用例子

## 代码
- 如果是段落上的一个函数或片段的代码可以用反引号把它包起来（`），例如：
```
`printf()` 函数
```
展示如下：
    `printf()` 函数
- 也可以用 ``` 包裹一段代码，并指定一种语言（也可以不指定）：
>\``` js
>$(document).ready(function () {
>    alert('BruceFc');
>});
>\```

  展示如下：
``` js
$(document).ready(function () {
    alert('BruceFc');
});
```

## 链接
- 链接使用方法为：
```
[链接名称](链接地址 'title')
或者
<链接地址>
```
例如：
```
[BruceFc](https://brucefc.github.io/ 'brucefccccccc')
或者
<https://brucefc.github.io/>
```
    **展示如下：**
    [BruceFc](https://brucefc.github.io/ 'brucefccccccc')
    或者
    <https://brucefc.github.io/>

## 图片
- Markdown 图片语法是在链接的基础上，前面加上`!`，格式如下：
```
![alt 属性文本](图片地址)
![alt 属性文本](图片地址 "可选标题")
```

## 表格
- Markdown 制作表格使用 `|` 来分隔不同的单元格，使用 `-` 来分隔表头和其他行。语法格式如下：
```
表头|表头|表头
:-|:-:|-:
内容|内容|内容
内容|内容|内容
```
展示如下：
表头|表头|表头
:-|:-:|-:
内容|内容|内容
内容|内容|内容
  - `-:` 设置内容和标题栏居右对齐。
  - `:-` 设置内容和标题栏居左对齐。
  - `:-:` 设置内容和标题栏居中对齐。

## 其他技巧
1. 支持的 HTML 元素
不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。目前支持的 HTML 元素有：`<kbd>` `<b>` `<i>` `<em>` `<sup>` `<sub>` `<br>`等 ，如：
```
使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑
```
展示如下：
键入 <kbd>quit</kbd> 来退出程序，或者键入 <kbd>menu</kbd> 来返回主菜单。

2. 转义
Markdown 使用了很多特殊符号来表示特定的意义，如果需要显示特定的符号则需要使用转义字符，Markdown 使用反斜杠转义特殊字符：
```
**文本加粗** 
\*\* 正常显示星号 \*\*
```
输出结果：
  **文本加粗** 
  \*\* 正常显示星号 \*\*

3. 高级链接
我们可以通过变量来设置一个链接，变量赋值在文档末尾进行：
```
这个链接用 1 作为网址变量 [Google][1]
这个链接用 baidu 作为网址变量 [Baidu][baidu]
然后在文档的结尾为变量赋值（网址）

  [1]: http://www.google.com/
  [runoob]: http://www.baidu.com/
```
以上语法输出结果为(变量赋值的内容被执行了，并未展示)：
这个链接用 1 作为网址变量 [Google][1]
这个链接用 baidu 作为网址变量 [Baidu][baidu]
这个链接用 BruceFc 作为网址变量 [BruceFc][BruceFc]
然后在文档的结尾为变量赋值（网址）

  [1]: http://www.google.com/
  [baidu]: http://www.baidu.com/
  [BruceFc]: https://brucefc.github.io/
