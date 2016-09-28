# 初识Atom(11)Themes —— 主题设置修改

关于主题，Atom自带了几套主题，当然用户可以自行下载自己喜欢的主题，要自己写一套主题，那是相当大的一个工程量~，Atom上已经有很多大神上传的主题，今天就以seti主题来说明。

> PS 说这个主题只是为了演示安装主题，以及修改主题样式设置，本人其实更偏好Atom自带的`one Dark`的`ui`及`syntax`主题~，这个风格更适合我的胃口~ 我觉得很赞的一点是代码着色方面，就如markdown文件标题和文本有不同着色，HTML文件标签的尖括号和标签英文有不同着色，这样看着比全篇一色的更舒服~

在`settings` -> `install`中搜索`seti` 点击搜索框右侧的`Themes`，其有`UI`主题，和`syntax`语法主题。

![][1]

两个插件包都安装上，进入`settings` -> `Themes`界面，选择UI主题以及`syntax`主题为`seti`。

![][2]

选择之后立马就可以看到效果~, 当然所有主题都有可能有一部分是自己不喜欢的，没问题，可以自己修改，还记得之前说到的开发者工具吗？ 这里就能用得到啦~！按`F12`打开开发者工具，想改哪一块，直接查找相关代码，将控制代码复制出来，打开`File` -> `Stylesheet...`文件。

我们对该编辑器所有样式上的调整，修改的代码都会写在这个文件中。

现在我想修改`tab`标签栏的高度以及标题的字体大小，开发者工具发现控制他的高度的有以下这些代码：

```
标签栏整体高度：
atom-workspace-axis.vertical .tab-bar{
    height: 60px;
}
标签tab高度：
atom-workspace-axis.vertical .tab-bar .tab{
    height: 60px;
    padding: 17px 10px;
}
标签tab字体大小：
.tab-bar .tab{
    font-size: 11px;
}
当前标签栏高度：
atom-workspace-axis.vertical .tab-bar .tab.active{
    height: 60px;
}
标签栏关闭按钮位置：
atom-workspace-axis.vertical .tab-bar .close-icon{
    top: 22px;
}

项目文件夹高度：
atom-panel-container .project-root > .header{
    height: 60px;
    padding: 15px 0 0 8px;
}
```

以上为所有控制标签栏的代码，当然，这里只列出了需要修改项，如果想要修改背景色什么，也可以将其复制出来，将这些代码粘贴进`Stylesheet...`文件，并经具体数值，改成自己偏好即可:

![][3]

这是修改后的效果，可以对比与上图的区别~，只要是由代码控制，在这里都可以进行修改~！

***
[1]:https://github.com/kaivin/atom/raw/master/images/seti/seti.png "seti主题"
[2]:https://github.com/kaivin/atom/raw/master/images/seti/seti1.png "seti主题"
[3]:https://github.com/kaivin/atom/raw/master/images/seti/seti2.png "seti主题"
