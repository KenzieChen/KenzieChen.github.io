---
layout: post
title: markdown和pygments的使用
category: 实用
tags: [markdown]
excerpt: 我用github和jekyll建立了自己的博客站点，用Markdown语法和pygments高亮写博客，直接用一些简单的标签，利用本地编辑器进行文本编辑，在本地调试预览，编辑完成后发布到github上，省去了在线博客排版，实现简单高效的博客编辑。
---
我用`github`和`jekyll`建立了自己的博客站点，用`Markdown`语法和`pygments`高亮写博客，直接用一些简单的标签，利用本地编辑器进行文本编辑，在本地调试预览，编辑完成后发布到`github上`，省去了在线博客排版，实现简单高效的博客编辑。

以下是对Markdown和pygments的测试：

标题一
======

标题二
------

###标题三

####标题四

#####标题五

######标题六

####有序列表（子列表相对父列表三个空格缩进）:

1. 列表1
   1. 列表1-1
   1. 列表1-2
      1. 列表1-2-1
      1. 列表1-2-2
1. 列表2
1. 列表3

####无序列表（子列表相对父列表两个空格缩进）：

* 列表1
  * 列表1-1
  * 列表1-2
    * 列表1-2-1
    * 列表1-2-2
* 列表2
* 列表3

####加粗和斜体(星号*或下划线_)

一个\*号包围是*斜体*

两个\*号包围是**粗体**

三个\*号包围是***粗斜体***

####引用（可以嵌套其他语法，包括包括引用、标题、列表、代码区块等）

> 我是第一段引用
>
>> 我是嵌套在第一段中的引用
>
> 我是第二段引用
>
>1. 引用区的列表1
>1. 引用区的列表2

####超链接

第一种链接方式（行内式）：[点我跳转到百度](http://www.baidu.com "百度")

第二种链接方式（参考式）：[点我跳转到百度][link]

[link]: http://www.baidu.com

第三种连接方式（隐式）：[点我跳转到百度][]

[点我跳转到百度]: http://www.baidu.com

第四种链接方式（自动,也可以是邮箱）：<http://www.baidu.com>

###图片，与超链接类似
--------------------------------------------------------------------我的logo--------------------------------------------------------------------------------

![我的logo](/kzlog.png "KenzieChen")

####代码区（缩进 4 个空格或是 1 个制表符）,在代码区块里面， & 、 < 和 > 会自动转成 HTML 实体，代码区块中，一般的 Markdown 语法不会被转换，像是星号便只是星号。
	this is code area
	<div class="footer">
        &copy; 2004 Foo Corporation
    </div>
    * 不是列表1
    * 不是列表2

上面代码区中的div中的内容如果不在代码区就会变成下面这样：

<div class="footer">
        &copy; 2004 Foo Corporation
</div>

####使用重音符号\`this is code\`来标记代码

`this is code`

####分隔线(三个以上的星号、减号、底线)

***
---
___

####pygments代码高亮

{% highlight java %}
//A test class
public class Kenzie{

  private String name;
  private String occupation;
  public static void main(Stirng[] args){
    name="Kenzie";
    occupation="Studeng";
    System.out.println("Name:"+name);
    System.out.println("Occupation:"+occupation);
  }
}
{% endhighlight %}