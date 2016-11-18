# 初识Atom(12) —— 插件推荐篇

本章将主要列出一些前端实用插件，当然，也包括那些让别人看到后会让他们感到你是很酷的插件~ 无形装逼最致命~！！

> 当然所有插件在安装前，必须确保电脑已经安装了node.js，且配置好node.js环境, .atom很多插件都是基于node.js做的。

## 前端依赖篇

| 插件 | 作用 | 备注 |
| :----- | :---- | :----- |
| [simplified-chinese-menu][1] | Atom的简体中文语言包，完整汉化，兼容所有已发布的版本Atom。 | 将装逼进行到底~我们就用英文版~ |
| [linter][2] | 该插件是用jshint来检查代码必须和`linter-jshint`组合实用，`linter-jshint`是依赖linter插件来使用的，也就是说必须先安装`linter`插件；因为`linter`是一个粗糙的检查，有很多针对专门项的代码检查，如`linter-csslint`、`linter-php`等等 | 还有`linter-scss-lint`,`linter-less`,`linter-coffeelint`等 |
| [emmet][3] | 它使用仿CSS选择器的语法来生成代码，大大提高了HTML/CSS代码编写的速度 | 神器！后期会有单章讲解 |
| [autoclose-html][4] | 自动补全HTML的结束标签，触发键为`>` | 也就是一对标签当写出开头标签的'>'时，会自动补全结束标签，且块状元素会自动换行并中间留空一行 |
| [atom-ternjs][5] | 该插件能对一个对象中拥有的对外提供的属性和方法都能通过suggest的形式提示出来，能对一个对象对外提供的接口有一个选择过程，可以理解为js代码自动提示。 | 智能提示JS代码~ |
| [platformio-ide-terminal][6] | atom内置终端工具 | 可在编辑器中打开并使用的命令行工具 |
| [autocomplete-paths][7] | 文件路径自动提示 | 自动提示有很多，Atom已经集成的`autocomplete-html`,`autocomplete-css`等 |
| [atom-beautify][8] | 美化代码的插件，几乎支持所有主流的语言 | 代码没有制表符缩进的可以通过这个格式化，让代码有层次感 |
| [jquery-snippets][9] | JQ代码块 | 也有其他的代码块如`css-snippets`,`es6-snippets`等等 |
| [autoprefixer][10] | 浏览器兼容 | 自动添加多浏览器兼容前缀 |
| [color-picker][11] | 拾色器 | 在编辑器中打开拾色器，随心所欲选择色值 |
| [docblockr][12] | 注释插件 | 有了这个插件，你仅仅需要一个tab键就可以写出专业的注释！ |
| [project-manager][13] | 管理项目 | 多项目通过该插件进行管理 |
| [project-viewer][32] | 管理多项目 | 多项目之间随意切换，不用再多开N个窗口了~ |
| [highlight-selected][33] | 高亮当前文档中所有和当前选中项相同的项 | IDE标配~ |

## 界面美化篇

| 插件 | 作用 | 备注 |
| :----- | :---- | :----- |
| [file-icons][14] | 增加许多图标,在侧边蓝文件名前面的icon | 每种文件都有一个专属小图标 |
| [tree-view-finder][15] | 左边菜单栏显示方式，类似Mac OS下的finder | 感觉不实用~ 压缩了工作区空间~ |
| [expose][16] | 多个打开的文件通过该方式可以全屏列出供选择 | 非常高大上的插件 |

## 前端协作篇

| 插件 | 作用 | 备注 |
| :----- | :---- | :----- |
| [grunt-runner][17] | 可以直接在编辑器里面操作grunt任务 | grunt想必都知道的~ |
| [bottom-dock][18] | 不仅仅可以实现gulp面板,还能实现todo[很实用的功能],还有grunt队列也能实现 | gulp必备插件 |
| [gulp-manager][19] | 与`bottom-dock`联合使用，缺一不可 | gulp必备插件 |
| [git-plus][20] | 提供git版本控制操作的命令 | 个人刚接触git，对这个不太熟悉，不做评价 |
| [git-status][34] | 文件状态管理查询 |  |
| [git-control][35] | git的命令按钮化 | 包括比较、提交、撤销、获取、拉取、推送、合并、分支、版本等 |
| [git-diff][36] | 比较文件不同的地方 |  |
| [git-history][37] | 可以查看历史版本文件 | 会另打开一个历史文件供查看 |
| [git-time-machine][38] | 可打开一个提交历史的时间图形界面 | 每一次的历史提交时间相当于一个点，点击图形中的点可查看当次历史提交的记录文件 |
| [git-log][39] | 图形化分之及提交历史 | 能用不同颜色区分不同分支，以及每次提交的描述、提交ID、日期、作者等。以列表形式展现 |
| [language-git][40] | 让atom支持git语言 | atom安装时应该已经集成了这个插件 |

## 操作增强篇

| 插件 | 作用 | 备注 |
| :----- | :---- | :----- |
| [minimap][21] | 右侧显示当前文件缩略图 | 与sublime text一样的东西~ 当然还能进行扩展 |
| [vim-mode][22] | vim党，一定会喜欢这个插件！ | 键盘操作，可能会有很多快捷键冲突，就需要自己一个一个修改啦~ |
| [sync-settings][31] | 插件、快捷键绑定备份 | 是一个为自己配置的atom进行备份的插件（配置的插件、样式、快捷键绑定等等），需要用到 `github` 上的 `Gist` 而 `Gist` 必须翻墙~ |

### minimap扩展

| 插件 | 作用 | 备注 |
| :----- | :---- | :----- |
| [minimap-codeglance][23] | 鼠标移动到缩略图上的时候放大显示那边部分的代码 | 与webstorm一样的东西~ |
| [minimap-find-and-replace][24] | 可以在缩略图上看到所有你选中的字符串 | 查找替换`ctrl+d`，当你想替换单词时，缩略图显示所有你选中的单词 |
| [minimap-git-diff][25] | 每当你修改你的代码的时候你就会在缩略图上看到和之前git中的区别 | git相关 |
| [minimap-highlight-selected][26] | 当你选中部分代码的时候，它就会高亮的出现在缩略图中 | 配合 `highlight-selected` 使用，绝配 |
| [minimap-linter][27] | 让你的缩略图显示的更加漂亮和完整 | 没用过~不太清楚~哈哈 |

## 主题推荐篇

| 插件 | 作用 | 备注 |
| :----- | :---- | :----- |
| [atom-material-ui][28] | UI主题 | 从atom上该插件的下载量可看出该插件的受欢迎程度~ |
| [atom-material-syntax][29] | 与上方的UI主题一组的语法主题 | 配套食用更健康~ |

## 强行装逼篇

| 插件 | 作用 | 备注 |
| :----- | :---- | :----- |
| [activate-power-mode][30] | 输入代码编辑器抖动，且会在光标上面飘出雪花一样的小方块~根据语法着色，显示不同颜色 | 这个效果太6了~ zhuangbility~ |


***

[1]:https://atom.io/packages/simplified-chinese-menu "simplified-chinese-menu"
[2]:https://atom.io/packages/linter "linter"
[3]:https://atom.io/packages/emmet "emmet"
[4]:https://atom.io/packages/autoclose-html "autoclose-html"
[5]:https://atom.io/packages/atom-ternjs "atom-ternjs"
[6]:https://atom.io/packages/platformio-ide-terminal "platformio-ide-terminal"
[7]:https://atom.io/packages/autocomplete-paths "autocomplete-paths"
[8]:https://atom.io/packages/atom-beautify "atom-beautify"
[9]:https://atom.io/packages/jquery-snippets "jquery-snippets"
[10]:https://atom.io/packages/autoprefixer "autoprefixer"
[11]:https://atom.io/packages/color-picker "color-picker"
[12]:https://atom.io/packages/docblockr "docblockr"
[13]:https://atom.io/packages/project-manager "project-manager"
[14]:https://atom.io/packages/file-icons "file-icons"
[15]:https://atom.io/packages/tree-view-finder "tree-view-finder"
[16]:https://atom.io/packages/expose "expose"
[17]:https://atom.io/packages/grunt-runner "grunt-runner"
[18]:https://atom.io/packages/bottom-dock "bottom-dock"
[19]:https://atom.io/packages/gulp-manager "gulp-manager"
[20]:https://atom.io/packages/git-plus "git-plus"
[21]:https://atom.io/packages/minimap "minimap"
[22]:https://atom.io/packages/vim-mode "vim-mode"
[23]:https://atom.io/packages/minimap-codeglance "minimap-codeglance"
[24]:https://atom.io/packages/minimap-find-and-replace "minimap-find-and-replace"
[25]:https://atom.io/packages/minimap-git-diff "minimap-git-diff"
[26]:https://atom.io/packages/minimap-highlight-selected "minimap-highlight-selected"
[27]:https://atom.io/packages/minimap-linter "minimap-linter"
[28]:https://atom.io/packages/atom-material-ui "atom-material-ui"
[29]:https://atom.io/packages/atom-material-syntax "atom-material-syntax"
[30]:https://atom.io/packages/activate-power-mode "activate-power-mode"
[31]:https://atom.io/packages/sync-settings "sync-settings"
[32]:https://atom.io/packages/project-viewer "project-viewer"
[33]:https://atom.io/packages/highlight-selected "highlight-selected"
[34]:https://atom.io/packages/git-status "git-status"
[35]:https://atom.io/packages/git-control "git-control"
[36]:https://atom.io/packages/git-diff "git-diff"
[37]:https://atom.io/packages/git-history "git-history"
[38]:https://atom.io/packages/git-time-machine "git-time-machine"
[39]:https://atom.io/packages/git-log "git-log"
[40]:https://atom.io/packages/language-git "language-git"
