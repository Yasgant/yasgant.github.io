---
layout: post
title: 不会html等知识，如何搭建一个自己的网站？
---
搞这个公众号本来就是想分享一些不算很硬核但实用的东西，但是之前不务正业也没弄什么正经东西。正好前段时间接触了下网站，就想给大家分享下我接触到的两种搭建网站的方法。

​
一、Google Sites

（[sites.google.com](sites.google.com)）

优点：十分方便，简单易上手。

缺点：个性化程度较低，模板不够丰富。

![Google Sites ScreenShot](../../../assets/img/Blog/SiteShare/Google Sites Screenshot.png)

从给定的几个模板中选取一个后，就像制作ppt一样，利用Insert菜单中的工具将各种元素按照自己喜好添加到网页中。

Pages菜单可以调整网页的结构。

Themes菜单可以调整字体以及颜色。

傻瓜式操作，我就不多介绍了，相信大家都能快速上手。
 
点击右上角的publish后就可以在sites.google.com/view/[xxx] 看到自己的网站了。

&nbsp;

二、GitHub Pages

优点：个性化程度更高，模板更多。

缺点：设置较为复杂。
 
在GitHub里新建一个Repository，名字随意(推荐为: <你的用户名>.github.io )，其他的都不用动。

![GitHub Create Repo](../../../assets/img/Blog/SiteShare/GitHub Create Repo.png)

进到repo后在Settings -> Pages -> Choose a theme 里面选一个自己喜欢的模板，然后按照markdown文件格式编辑这个repo里的index.md 就可以更改网页内容了。
 
假如我的GitHub用户名是abc，那么就可以在abc.github.io这个网站看到自己设计的网页。如果我想要在abc.github.io/test里做一个新的网页，那么只需要在repo中新建test.md文件就可以。同理，如果想在abc.github.io/aaa/bbb显示内容，那么就需要新建一个aaa的文件夹，然后在文件夹里新建bbb.md就可以。

![GitHub Folder](../../../assets/img/Blog/SiteShare/GitHub Folder.png)

除了GitHub内置的那些模板外，我们还可以选择网络上的第三方模板，比如(http://jekyllthemes.org) 这个网站就提供了好多免费的模板。想要套用的话只需要进入到这个模板的GitHub Repo，选择Fork就可以把这个模板复制一份到自己的仓库里了。然后只需要编辑index.md或是其他文件就可以更改显示内容了。

![GitHub Fork](../../../assets/img/Blog/SiteShare/GitHub Fork.png)

注意：每次更改仓库里的文件后，大概需要一分钟才能在Pages网页上看到这次的更改。如果一分钟后没有看到网页，可以检查下Settings -> Pages -> Source -> Branch 有没有选择正确的分支，或者是markdown语法是否有错误。
 
如果想要个性化设置，比如更改字体，更改背景等等，可以查阅Jekyll的文档 (英文: [https://jekyllrb.com](https://jekyllrb.com) 中文: [https://www.jekyll.com.cn](https://www.jekyll.com.cn) (中文版文档内容不是很全))

&nbsp;

其他问题：

1. 什么是Markdown？

	Markdown是一种文本标记语言，你可以将它理解为代码化的word文档。如果不想使用加粗、表格、插入图片、插入数学公式等功能的话，直接用编辑txt文档的方式编辑markdown也是可以的。学习使用markdown的强大功能也不是很难，我推荐可以在Runoob ([https://www.runoob.com/markdown](https://www.runoob.com/markdown))了解一下这门语言。
 
2. 我不想使用sites.google.com/view/ 或是abc.github.io 作为我的网站域名，我怎么把网站域名改为别的呢？
 
	首先得先从域名提供商(Google Domains / 腾讯云 / 阿里云)购买一个域名，然后按照Google Sites / GitHub Pages 和域名提供商提供的步骤将自己的网站重定向至新的域名即可。另外Google Sites原先提供的域名在墙内是访问不到的，换了新的域名之后应该就可以从墙内访问到了。
