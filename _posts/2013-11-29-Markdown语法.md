#Markdown语法
2013-11-29 By Harx 整理自：[http://www.worldhello.net/gotgithub/appendix/markups.html#id50](http://www.worldhello.net/gotgithub/appendix/markups.html#id50)

关于Github的[GFM(Github Flavored Markdown)](https://help.github.com/articles/github-flavored-markdown)，以后再整理。

标题
-------

>一级标题
=========  

    # 一级标题
或

    一级标题
    ========
       
>## 二级标题

    ## 二级标题
或

    二级标题
    --------
>### 三级标题  

    ### 三级标题
    
>#### 四级标题    

    #### 四级标题
    
>##### 五级标题

    ##### 五级标题
    
>###### 六级标题 

    ###### 六级标题
    

    
段落
-------

**空行分段**

>第一段文字
    
>第二段文字

    第一段文字
    
    第二段文字

**自动续行**(但是两句间会有一个空格的空白。）

>一个回车不分段。（这里》
>《）本行续上行。

    一个回车不分段。（这里》
    《）本行续上行。
    
**插入换行**

>行尾两空格  
>保持换行。

    行尾两空格_ _  
    保持换行。
    
**段落缩进**

> 第一级段落缩进。
>
> > 第二级段落缩进。
>
> 返回一级段落缩进。

    
    > 第一级段落缩进。
    >
    > > 第二级段落缩进。
    >
    > 返回一级段落缩进。
      
    
**代码块**

四个空格缩进（或者两个tab）是代码块。（上边圈起来的都是）

>```
>code
>```

三个连续的`或~等符号界定代码块。gfm

>```ruby
>require 'redcarpet'
>md = Redcarpet.new("Hello, world.")
>puts md.to_html
>```

    ```ruby
    require 'redcarpet'
    md = Redcarpet.new("Hello, world.")
    puts md.to_html
    ```

列表（列表标记与条目间要有一个空格）
--------

**无序列表**

>* 星号、减号、加号开始列表。
>  - 列表层级和缩进有关。
>    + 和具体符号无关。
>* 返回一级列表。

```
* 星号、减号、加号开始列表。
  - 列表层级和缩进有关。
    + 和具体符号无关。
* 返回一级列表。
```

**有序列表**

>1. 数字和点开始有序列表。
>   1. 注意子列表的缩进位置。
>      1. 三级列表。
>      1. 编号会自动更正。
>   1. 二级列表，编号自动更正为2。
>2. 返回一级列表。

```
1. 数字和点开始有序列表。
   1. 注意子列表的缩进位置。
      1. 三级列表。
      1. 编号会自动更正。
   1. 二级列表，编号自动更正为2。
2. 返回一级列表。
```
    
**列表续行、段落和代码块**
    
>1. 列表项可以折行，
>   对齐则自动续行。
>2. 列表项可包含多个段落。
>
>    空行开始的新段落必须缩进四个空格，
>    段落才属于列表项。
>    
>3. 列表中的代码块要缩进8个空格。
>
>               $ printf "Hello, world.\n"    

```
1. 列表项可以折行，
   对齐则自动续行。
2. 列表项可包含多个段落。

    空行开始的新段落必须缩进四个空格，
    段落才属于列表项。
    
3. 列表中的代码块要缩进8个空格。

        $ printf "Hello, world.\n"  
```

分割线
--------

三条或更多短线（或星号、下划线）\
显示为分隔线。

>---

    ---

字体
----

>**粗体**

    **粗体**
    
>*斜体*

    *斜体*
    
>~~删除线~~gfm

    ~~删除线~~
    
><u>下划线</u> （GitHub无效果）

    <u>下划线</u>
    
>下标：H<sub>2</sub>O

    H<sub>2</sub>O
    
>上标：E = mc<sup>2</sup>

    E = mc<sup>2</sup>
    
>等宽字体：行内反引号嵌入代码，如: `git status` 。

    行内反引号嵌入代码，如: `git status` 。
    
链接
------

**URL自动链接**gfm

>网址 http://github.com/

>邮件 me@foo.bar

    网址 http://github.com/
    邮件 me@foo.bar
    
**文字链接**

>访问 [Google](http://google.com "Search")

>访问 [GitHub][1]

>访问 [WorldHello][]

[1]: http://github.com "Git host"
[worldhello]: http://www.worldhello.net

    - 访问 [Google](http://google.com "Search")
    - 访问 [GitHub][1]
    - 访问 [WorldHello][]
     [1]: http://github.com "Git host"
     [worldhello]: http://www.worldhello.net
    
**内部跳转**

<a name="md-anchor" id="md-anchor"></a>

>跳转至 [文内链接](#md-anchor) 。

    <a name="md-anchor" id="md-anchor"></a>
    跳转至 [文内链接](#md-anchor) 。

**GitHub提交和问题链接**gfm

>指向同一提交的链接：
>- 提交ID（SHA）: cea00609ca8...
>- 用户@提交ID: mojombo@cea00609ca8...
>- 用户名/项目名@提交ID:mojombo/god@cea00609ca8...

        指向同一提交的链接：
        - 提交ID（SHA）: cea00609ca8...
        - 用户@提交ID: mojombo@cea00609ca8...
        - 用户名/项目名@提交ID:mojombo/god@cea00609ca8... 

>指向同一Issue的链接：
>- Issue编号: #1
>- 用户名及Issue编号: mojombo#1
>- 用户名/项目名及Issue编号:mojombo/god#

        指向同一Issue的链接：
        - Issue编号: #1
        - 用户名及Issue编号: mojombo#1
        - 用户名/项目名及Issue编号:mojombo/god#1
    
图片
----------

![GitHub](/images/github.png "Logo")

    ![GitHub](/images/github.png "Logo")

GitHub Logo: ![GitHub][logo]
[logo]: /images/github.png "Logo"

    GitHub Logo: ![GitHub][logo]
    [logo]: /images/github.png "Logo"
    
表格gfm
-------

>head1 | head2  | head2
>------|:------:|------:
>left  | center | right
>left  | center | right

```
head1 | head2  | head2
------|:------:|------:
left  | center | right
left  | center | right
```   

    
其他
------

**混用HTML**

    <div style="background:#bbb;">
      HTML块中不能混用 **标记语法**
    </div>
    
    
    
    
    
    
