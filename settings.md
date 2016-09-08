# 设置中心
设置中心共分八大模块，本章将逐一进行讲解。

![][1]

`Open Config Folder`打开的是该软件的配置文件集合目录

# 目录
* [Core —— 核心](#核心)
* [Editor —— 编辑器设置](#编辑器设置)
* [System —— 系统设置](#系统设置)
* [Keybindings —— 快捷键](#快捷键)
* [Packages —— 包管理](#包管理)
* [Themes —— 主题管理](#主题管理)
* [Updates —— 更新](#更新)
* [Install —— 安装](#安装)

# 核心
顾名思义就是编辑器的一些核心设置，自动隐藏菜单栏、自动更新、自动关闭空窗口、自动关闭空的分屏的一些设置，这里不做详细讲解。

# 编辑器设置
这里主要针对的编辑窗口的设置，主要讲一下比较常用的一些：

* `Auto Indent` —— 自动缩进，也就是写代码时每一层级的标签都会比上一层级多一个缩进距离。
* `Auto Indent On Paste` —— 粘贴自动缩进，即粘贴进编辑窗口的代码也可自动进行层级缩进。
* 接下来的`Font Family`以及`Font Size`都可根据自己喜好进行设置，还有之后的`Line Height`同样如此。
* `Show Line Numbers` —— 显示行数，即编辑窗口的代表行数的数字。
* `Soft Wrap`以`Soft Wrap At Preferred Line Length`这两项如果要勾选，需都勾选才会起作用。其作用就是让编辑窗口内的内容在中线之前就换行，随便打开或新建一个文件窗口，可看见文件窗口的中间有条竖线，这两项勾选之后，每行内容长度只要超过这条线，就会自动换行。
* `Tab Length`这里默认会是两个空格键，一般来说，写代码会设置成4，即每次缩进4个空格。效果也作用于上文中所说的自动缩进。

> 此处的设置如用户做了自己的偏好设置，那么可以在`File-Config...`文件内找到相关修改

# 系统设置
这里都不需要明白，保持默认即可（其实我也不明白，大概意思是atom编辑器如何与用户的操作系统进行交互吧~）

# 快捷键
 快捷键配置,默认快捷键都汇总于此了,很方便查询对应的快捷键的功能,也方便修改

![][2]

# 包管理
插件管理中心,可以设置插件,删除插件及禁用,无安装功能

![][3]

![][6]

# 主题管理
主题管理中心,可以设置主题(支持鼠标选定,也支持写入配置文件生效),编辑器主题、语法主题等等

![][4]

![][7]

# 更新
所有插件安装包的可用最新版本状态，已安装的插件包如果有新版本可用，都在这里列出来，可在这里查看并更新

# 安装
可在这里搜索、安装`Package`和`Theme`,可在搜索条选择是搜索`Package`还是`Theme`。

![][5]

[1]:https://github.com/kaivin/atom/raw/master/images/settings/settings.png "设置中心"
[2]:https://github.com/kaivin/atom/raw/master/images/settings/keybindings.png "快捷键设置"
[3]:https://github.com/kaivin/atom/raw/master/images/settings/packages.png "包管理"
[4]:https://github.com/kaivin/atom/raw/master/images/settings/themes.png "主题管理"
[5]:https://github.com/kaivin/atom/raw/master/images/settings/install.png "安装包/主题"
[6]:https://github.com/kaivin/atom/raw/master/images/settings/package1.png "主题管理"
[7]:https://github.com/kaivin/atom/raw/master/images/settings/theme1.png "主题管理"
