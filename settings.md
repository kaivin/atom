# 初识Atom —— 设置
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
* 如果勾选了 `Soft Wrap` 选项，Atom 会在一行中的文本超出屏幕显示范围时将其折为两行，如果不勾选，过长的行将简单地超出屏幕显示范围，你必须要横向移动滚动条才能看到剩余的部分。如果 `Soft Wrap At Preferred Line Length` 选项被勾选，则总是会在 80 个字符处折行，你也可以设置一个自定义的长度来替换掉默认的 80 个字符。此长度即决定编辑窗口中间的分界线位置
* `Tab Length`这里默认会是两个空格键，一般来说，写代码会设置成4，即每次缩进4个空格。效果也作用于上文中所说的自动缩进。

> 此处的设置如用户做了自己的偏好设置，那么可以在`File-Config...`文件内找到相关修改

# 系统设置
这里都不需要明白，保持默认即可（其实我也不明白，大概意思是atom编辑器如何与用户的操作系统进行交互吧~）

# 快捷键
 快捷键配置,默认快捷键都汇总于此了,很方便查询对应的快捷键的功能,也方便修改。

![][2]

首先需要了解一下快捷键的组成，如图中共分四部分，快捷键(Keystroke) + 执行命令(Command) + 来源(Source) + 选择器(Selector)<br />
若要配置我们自己的快捷键，需要打开`File-Keymap...`文件，如下图：

![][8]

文件内我们需要注意的只是该图中，红框标注的部分，灰色显示的两个快捷键设置，为该软件给的示例设置方式，高亮的则为起作用的快捷键设置，前方不加`#`。基础的快捷键设置包含3个部分：
```
 'atom-text-editor':
    'enter': 'editor:newline'
```
- 第一行'atom-text-editor'是Selector（选择器）所代表的内容，即触发这个快捷键的区域
- 第二行'enter'是Keystroke（快捷键）所代表的内容，即按键
- 第二行'editor:newline'是Command（执行命令）所代表的内容，即要触发的命令（可以在 Ctrl+Shift+P 中看到准确的命令名）
- 三者之间都有一个`:`隔开
- 格式必须遵守如此的两行格式，以及第二行必须比上一行多一个缩进，否则会报错

具体的修改、添加、移除操作，可看本教程[初识Atom —— keymap快捷键设置][14]

# 包管理
插件管理中心,可以设置插件,删除插件及禁用,无安装功能

![][3]

![][6]

以上两张图片展示了包管理中，所包含的包的种类，共分四类：

1. community packages 社区包，主要是用户从atom社区下载并安装的包，会显示在这里。
2. core packeages 核心包，主要是atom自身集成的一些包，是这个编辑器的一些基本使用插件包，以及依赖包。
3. development packages 开发包，主要是项目开发依赖包，下载后，会显示在这里。
4. Git Packages Git包，目前不清楚哪些包会在这里列出，也许就是字面意思~。

此界面最上方的`Installed packages`也就是用户编辑器安装的所有包，和四个分类一样，后面都有计数。

> 那么这里主要需要说明的是：
  1. 可以通过搜索条搜索你要找的已安装的包
  2. 每个包的在这里显示的组成是：
    - 第一行左侧为包名/安装版本、右侧为下载量
    - 第二行是包的作者对这个包的描述
    - 第三行左侧显示包的作者、右侧有四项显示项，从做到右：
        - 更新版本 —— 这一项只在安装包出现新版本时会高亮显示出来
        - settings —— 设置，此项如果用户可以对该包进行自定义的设置，才会在这里显示，可点击，进行用户的自定义偏好设置
        - Uninstall —— 卸载，此项只在该安装包是编辑器允许卸载，即非编辑器本身依赖包时可显示，可将已安装包直接卸载
        - Disable —— 禁用，此项所有包基本都会显示，所有包都可以禁用，也都可以再次点击启用

# 主题管理
主题管理中心,可以设置主题(支持鼠标选定,也支持写入配置文件生效),编辑器主题、语法主题等等

![][4]

![][7]

主题这一块与上面所说的包基本一致，区别只在于这里多选择主题的区块。其核心主题列表中，atom已经自带了很多种主题，当然在最上方的UI主题以及Syntax主题都可以自主进行选择。

# 更新
所有插件安装包的可用最新版本状态，已安装的插件包如果有新版本可用，都在这里列出来，可在这里查看并更新

![][12]

更新除了在上述所说，包/主题列表中显示出有新版本。已安装的包/主题所有有新版本时，也都将在这里列出来，用户可以通过某一个包/主题上的更新按钮来更新单个插件，也可以直接通过该界面上的`Update All`来更新全部插件。

# 安装
可在这里搜索、安装`Package`和`Theme`,可在搜索条选择是搜索`Package`还是`Theme`。

![][5]

如上图，这里会列出所有在atom官网上已有的包/主题,可以通过搜索来找到用户需要的包，点击`install`即可进行安装。

当然也许你会遇到麻烦：怎么都安装不上，或者这里没有搜到你想要的包，总之就是，你无法通过点击`install`的方式安装你需要的那个包，那么你可以访问我的这篇文章——[初识Atom —— package安装方法总结][13]

***

[1]:https://github.com/kaivin/atom/raw/master/images/settings/settings.png "设置中心"
[2]:https://github.com/kaivin/atom/raw/master/images/settings/keybindings.png "快捷键设置"
[3]:https://github.com/kaivin/atom/raw/master/images/settings/packages.png "包管理"
[4]:https://github.com/kaivin/atom/raw/master/images/settings/themes.png "主题管理"
[5]:https://github.com/kaivin/atom/raw/master/images/settings/install.png "安装包/主题"
[6]:https://github.com/kaivin/atom/raw/master/images/settings/package1.png "主题管理"
[7]:https://github.com/kaivin/atom/raw/master/images/settings/theme1.png "主题管理"
[8]:https://github.com/kaivin/atom/raw/master/images/settings/keymap.png "keymap文件"
[9]:/menuBar.md "菜单栏"
[10]:https://github.com/kaivin/atom/raw/master/images/settings/keymap1.png "keymap文件"
[11]:https://github.com/kaivin/atom/raw/master/images/settings/keymap2.png "keymap文件"
[12]:https://github.com/kaivin/atom/raw/master/images/settings/update.png "更新包/主题"
[13]:/packages.md "包安装"
[13]:/keymap.md "快捷键设置"
