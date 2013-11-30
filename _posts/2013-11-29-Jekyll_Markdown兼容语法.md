---
layout: default
---

#Jekyll_Markdown兼容语法
2013-11-29 By Harx

标题
-------

>#一级标题

    # 一级标题
       
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
        
>下标：H<sub>2</sub>O

    H<sub>2</sub>O
    
>上标：E = mc<sup>2</sup>

    E = mc<sup>2</sup>
    
>等宽字体：行内反引号嵌入代码，如: `git status` 。

    行内反引号嵌入代码，如: `git status` 。
    
链接
------

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


		head1 | head2  | head2
		------|:------:|------:
		left  | center | right
		left  | center | right
    
其他
------

**混用HTML**

    <div style="background:#bbb;">
      HTML块中不能混用 **标记语法**
    </div>
