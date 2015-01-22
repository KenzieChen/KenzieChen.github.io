---
layout: post
title: "测试页面"
category: 测试
tags: [helloworld, markdown, showcase]
excerpt: >
  使用Jekyll搭建了一个个人博客，用Markdown语法写博客。下面是一些测试用的语法示例。
---
  使用Jekyll搭建了一个个人博客，用Markdown语法写博客。下面是一些测试用的语法示例。

标题一
================

标题二
----------------

### 标题三

#### 标题四

##### 标题五

###### 标题六

有序和无序列表
------------

**有序列表:**

1. 项目1
1. 项目2
1. 项目3

**无序列表：**

* 项目1
  + 项目1-1
    - 项目1-1-1
* 项目2
* 项目3

加粗和斜体
-----------

这个应该是**粗体**,__这个也是粗体__，这是*斜体*，这是***粗斜体***。

> 这个是引用

超链接和图片
------------

从[Jekyll的官方网站](http://jekyllrb.com/) 可以查到一些很有很有帮助的文档。
但是[JekyllBootstrap](http://jekyllbootstrap.com/) 虽然在Jekyll基础上做了很多工作但是官方网站样式并不漂亮，并且JekyllBootstrap本身也貌似很久没更新了的样子。

### 我的logo
![我的logo](/kzlog.png "KenzieChen")

`this is code`

### 代码高亮，采用的是pygments


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
