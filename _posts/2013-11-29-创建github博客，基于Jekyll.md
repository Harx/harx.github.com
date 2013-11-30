---
layout: default
title: 创建github博客，基于Jekyll
---

###1. github上创建仓库，命名为USERNAME.github.com

注意勾选初始化并创建README.md的选项，这样就不用再折腾本地初始化了。

###2. 初始化后，进入仓库设置页面，找到'GitHub Pages'下的'automatic page generator'，点击自动生成。之后按步骤设置。

###3. 创建_layouts（放主题）,_posts（放文字）目录。

###4. 自己设置主题模板，修改_layouts文件夹里的default.html文件。

这里，使用bootstrap进行页面构建。简洁、响应式。

###5. 添加文章。在_posts文件夹里创建文本文档，修改名字和扩展名为YEAR-MONTH-DAY-TITLE.md。
如果需要jekyll解析，则开头必须包含YML代码。

