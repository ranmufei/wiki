> wiki 支持两种语法格式
>> 1 markdown  参考语法 http://equation85.github.io/blog/markdown-examples/

## 语法测试工具
* http://maxiang.info/

>> 2 Rdoc 


----       = 创建水平线.
\\         = 换行, \\\=force line break and clear.

> ## 这是一个标题。
> 
> 1.   这是第一行列表项。
> 2.   这是第二行列表项。
> 
> 给出一些例子代码：
> 
>     return shell_exec("echo $input | $markdown_script");

# wiki帮助文档

[link]     = 创建一个链接，指向内部的wiki页面'Link'.
[this is also a link] = 创建一个链接，指向内部的wiki页面'ThisIsAlsoALink'.
[click here|link] = 创建一个链接，指向内部的wiki页面'Link', 链接文字是'click here'.
[1]        = Makes a reference to a footnote numbered 1.
[#1]       = Marks the footnote number 1.
[[link]    = 不创建链接而是输出文字'[link]'.

## 大小标题

!heading   = 小号标题
!!heading  = 中号标题
!!!heading = 大号标题

''text''   = 将text斜体.
__text__   = 将text粗体.
{{text}}   = prints 'text' in monospaced font.

* text     = 无符号列表
# text     = 有符号列表
什么是Markdown

Markdown是一个将文本转化为HTML的工具。简单来说，Markdown是一个兼顾可读性与易用性的轻量级标记体系。Markdown并不追求大而全，它只关心HTML里最常用的几个标记，对于一些不常用的标记它允许直接将HTML标记插入文本。

标题

Markdown提供了两种方式（Setext和Atx）来显示标题。

语法：

Setext方式
标题1
=================

标题2
-----------------

Atx方式
# 标题1
## 标题2
###### 标题6
效果：

Setext方式

标题1

标题2

Atx方式

标题1

标题2

标题6

换行

在文字的末尾使用两个或两个以上的空格来表示换行。

引用

行首使用>加上一个空格表示引用段落，内部可以嵌套多个引用。

语法：

> 这是一个引用，
> 这里木有换行，   
> 在这里换行了。
> > 内部嵌套
效果：

这是一个引用， 这里木有换行，
在这里换行了。

内部嵌套

列表

无序列表使用*、+或-后面加上空格来表示。

语法：

* Item 1
* Item 2
* Item 3

+ Item 1
+ Item 2
+ Item 3

- Item 1
- Item 2
- Item 3
效果：

Item 1
Item 2
Item 3

Item 1

Item 2

Item 3

Item 1

Item 2

Item 3

有序列表使用数字加英文句号加空格表示。

语法：

1. Item 1
2. Item 2
3. Item 3
效果：

Item 1
Item 2
Item 3
代码区域

行内代码使用反斜杠`表示。
代码段落则是在每行文字前加4个空格或者1个缩进符表示。

语法：

Bash中可以使用echo来进行输出。
    $ echo 'Something'
    $ echo -e '\tSomething\n'
效果：

Bash中可以使用echo来进行输出。

$ echo 'Something'
$ echo -e '\tSomething\n'
强调

Markdown使用\*或\_表示强调。

语法：

单星号 = *斜体*
单下划线 = _斜体_
双星号 = **加粗**
双下划线 = __加粗__
效果：

单星号 = 斜体
单下划线 = 斜体
双星号 = 加粗
双下划线 = 加粗

链接

Markdown支持两种风格的链接：Inline和Reference。

语法：

Inline：以中括号标记显示的链接文本，后面紧跟用小括号包围的链接。如果链接有title属性，则在链接中使用空格加"title属性"。
Reference：一般应用于多个不同位置使用相同链接。通常分为两个部分，调用部分为[链接文本][ref]；定义部分可以出现在文本中的其他位置，格式为[ref]: http://some/link/address (可选的标题)。
注：ref中不区分大小写。

这是一个Inline[示例](http://equation85.github.com "可选的title")。
这是一个Reference[示例][ref]。
[ref]: http://equation85.github.com
效果：

这是一个Inline示例。
这是一个Reference示例。

图片

图片的使用方法基本上和链接类似，只是在中括号前加叹号。
注：Markdown不能设置图片大小，如果必须设置则应使用HTML标记<img>。

语法：

Inline示例：![替代文本](/assets/images/jian.jpg "可选的title")
Reference示例：![替代文本][pic]
[pic]: /assets/images/ship.jpg "可选的title"
HTML示例：<img src="/assets/images/jian.jpg" alt="替代文本" title="标题文本" width="200" />
效果：

替代文本

其他

自动链接

使用尖括号，可以为输入的URL或者邮箱自动创建链接。如test@domain.com。

分隔线

在一行中使用三个或三个以上的*、-或_可以添加分隔线，其中可以有空白，但是不能有其他字符。

转义字符

Markdown中的转义字符为\，可以转义的有：

\\ 反斜杠
\` 反引号
\* 星号
\_ 下划线
\{\} 大括号
\[\] 中括号
\(\) 小括号
\# 井号
\+ 加号
\- 减号
\. 英文句号
\! 感叹号
结语

Markdown语法很大程度上减少了编辑的成本，但是在写作这篇文章的时候也发现某些标记对中文的支持似乎并不完美，虽然这些缺陷可以通过直接插入HTML代码解决（但这么做一点都不漂亮）。总的来说，能够在离线状态下使用命令行模式进行写作还是很爽的，相比在线写作模式精力可以更专注。

#### tips（陈孔毅新加）:
wiki里面标注已解决可以这样实现，分享下 ：  
>   ___[【已解决】](#)___ 
>  ` ___[【已解决】](#)___ 
>  把上面的复制到标题前面就可以了