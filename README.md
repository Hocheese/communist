# 共产主义文档
现在网上能够在线浏览马列主义经典著作的网站用户体验都太差，所以我计划用hexo做一个展示马列主义经典著作的站点。
而且以前我接触到的马列主义思想都是碎片化的，所以我打算借此机会读一读这些经典文章。

欢迎志同道合的同志们加入。[演示地址](http://marx.largeq.cn)

### 编辑说明

所有文档来源来自社科院的[资料库](http://clas.cssn.cn/sjxz/xsjdk/mkszyjd/)。我本来想直接录入马恩全集的，但是事实证明编辑工作并不只是简单的复制粘贴然后再做一个模板。现在互联网上公开的马列主义经典 差劲的阅读体验 不仅仅来自于各个资料库所采用的远古时代的web技术，还来自于为纸质书设计的排版格式，比如正文中出现的注释、时不时出现的“第N页”。

所以我决定先编辑好马列选集第一卷的部分文章，以便调试程序，然后再做一个本文档专用的主题。最好还能编写一个自动化脚本把社科院的选集批量下载下来，然后自动转成markdown。我可能还需要自己编写一个hexo插件来优化这些为纸质书设计的注释。
### 最新章节
哲学的贫困
### 待进行的工作列表
* 制作一个本站专属主题
* 找到处理注释与页码的解决方案
    * 注释怎么处理（我希望它能够通过汽泡来显示）
    * 页码怎么处理（是否需要以此来制作分页效果）
    * 作者怎么显示（作者可能是马克思，恩格斯，马克思与恩格斯）
* 编写一个自动下载文章并转成md格式的脚本
* 运行脚本并进行校对，处理乱码
### 如何添加文章
添加文章没必要像hexo官网介绍的那样用指令，直接在source/_posts下新建文件（夹），在文件头部插入:

~~~
---
title: 马克思《黑格尔法哲学批判》导言
categories: 马恩选集第一卷
tags: [马克思,黑格尔]
---
~~~

然后写入文章内容，执行 `hexo clean` 和 `hexo generate` 就可以了。