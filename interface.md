
# 目录
* [初始界面](#初始界面)
* [菜单栏](#菜单栏)
    * [File(文件)](#File —— 文件)
    * [Edit(编辑)](#Edit —— 编辑)
    * [View(视图)](#View —— 视图)
    * [Selection(选择)](#Selection —— 选择)
    * [Find(查找)](#Find —— 查找)
    * [Packages(包)](#Packages —— 包)
    * [Help(帮助)](#Help——帮助)

***

# 初始界面
当你第一次打开 Atom 的时候，你会看到这样的一个窗口：

![][1]

这是 Atom 的欢迎屏幕（welcome screen），它展示了一些不错的建议，帮助你了解 Atom.<br />
此界面可大致分为上（菜单栏）、中（操作窗口）、下（状态栏）三大块，下面我们先通过菜单栏来逐步了解Atom.

# 菜单栏
1. File — 文件 文件的保存打开,项目的保存打开,最后一次的项目加载,关闭及设置中心,以及用户自定义的配置(配置文件,初始化脚本,样式风格,代码片段,快捷键配置文件)等
2. Edit — 编辑 文件编辑的操作,文件编码格式,及行跳转等
3. View — 视图 重载页面,全屏,字体大小的缩放等
4. Selection — 选择 光标选择项等
4. Find — 查找 都是关于查询的 ,跟Sublime text极其相似,快捷键基本一样
5. Packages — 包 就是插件列表的集合点
6. Help — 帮助 帮助文档、软件更新、协议等

## File —— 文件
点击File弹出的菜单可以看到被分割线分为了六大块

### 1. 文件操作项
这一部分都是常规操作，不做详细描述。

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+Shift+N | New Window | 新窗口 | 新建一个Atom窗口 |
| Ctrl+N | New File | 新建文件 | 如中文 |
| Ctrl+O | Open File... | 打开文件 | 如中文|
| Ctrl+Shift+O | Open Floder... | 打开文件夹 | 如中文 |
| Alt+Ctrl+O | Add Project Floder... | 添加项目文件夹 | 添加的为项目的根目录文件夹 |
| Ctrl+Shift+T | Reopen Last Item | 重新打开最后关闭的那一项 | 如中文 |

### 2. Settings —— 设置中心
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+Comma | Settings | 设置中心 | 打开设置中心`Comma`即`逗号`
 |
> 此快捷键并未起作用，问题可看本文档[Settings View —— 设置中心视图](#Settings View —— 设置中心视图)<br />
Settings的内容为用户对这个编辑器的个人偏好设置，这个会在另一篇文章-[设置][2]中进行详细介绍。

### 3. 个人配置文件
这一块主要是个人偏好配置需要修改的文件。

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :---- | :---- |
|  | Config... | 配置 | 用户对这个编辑器做了任何改动都可以在这里找到相关信息 |
|  | Init Script... | 初始化脚本 |  |
|  | Keymap... | 键盘模式 | 即快捷键设置，如果编辑器的自身的快捷键你用着不习惯，可以在这里设置成你喜欢的快捷键，具体设置方法会在[设置][2]中讲到 |
|  | Snippets... | 代码块 | 可以在这里预设一个代码块，通过输入在这里设置的一个超短命令后，按`tab`键，达到瞬间输出你在这里所设置的代码块的目的 |
|  | Stylesheet... | 样式表 | 在设置中，用户对这个编辑器本身的样式做了修改后，所修改的样式都会在这里出现 |

### 4. 保存
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+S | Save | 保存 | 如中文 |
| Ctrl+Shift+S | Save As... | 另存为... | 如中文 |
| Save All... | 保存全部 | 项目中所有经过修改未保存的文件，都会被保存 |

### 5. 关闭选项
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+W | Close Tab | 关闭选项卡 | 关闭当前选项卡，即关闭用户当前所在的文件窗口 |
|  | Close Pane | 关闭窗格 | 当用户将编辑器进行[分屏操作][3]后，可通过点击此项来关闭当前分屏 |
| Ctrl+Shift+W | Close Window | 关闭窗口 | 即关闭当前打开的Atom编辑器 |

### 6. 退出
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :----- | :---- | :---- |
|  | Exit | 退出 | 点击此键后，会退出该软件，即如果用户打开了很多项目，每个项目都是一个新窗口编辑器，那么此操作过后，所有打开的编辑器都将被关闭 |
|  | Close ALL Tabs | 关闭所有选项卡 | 关闭所有被打开的选项卡 |

## Edit —— 编辑
此菜单栏内，均是针对文件的操作的选项：

### 1. 撤销重做
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+Z | Undo | 撤销 | 撤销上一次操作 |
| Ctrl+Z | Redo | 重做 | 重做上一次操作 |

### 2. 复制黏贴
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+X | Cut | 剪切 | 如中文 |
| Ctrl+C | Copy | 复制 | 如中文 |
| Ctrl+Shift+C | Copy Path | 复制路径 | 如中文 |
| Ctrl+V | Paste | 粘贴 | 如中文 |
| Ctrl+A | Select All | 全选 | 如中文 |

### 3. 其他
#### 单项
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+/ | Toggle Comments | 添加注释 | 可根据文件格式智能选择何种注释符 |
| Alt+Ctrl+Q | Reflow Selection | 浮动选择区域 | 测试效果为光标所在的行追加到其上一行的后面 |
| Ctrl+Shift+U | Select Encoding | 选择文件编码格式 | 如中文 |
| Ctrl+G | Go to Line | 跳转到某行 | 可跳转到行，也可跳转到某行的某列位置，语法row:columns。例：20:30——>20行30列 |
| Ctrl+Shift+L | Select Grammar | 选择语法格式 | 给文件选择一种语言格式，也就是什么后缀的文件 |

#### Lines 行
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+] | Indent | 缩进 | 光标所在行缩进，其效果如同`Tab`,区别在于光标在行的任何位置，此快捷键都是缩进此行，而非光标在哪里就从哪里缩进 |
| Ctrl+[ | Outdent | 回退缩进 | 撤销通过`Ctrl+]`产生的缩进 |
|  | Auto Indent | 自动缩进 | 无测试效果 |
| Ctrl+Up Arrow | Move Line Up | 光标所在行上移一行 | 如中文 Up Arrow即鍵盤上的上箭頭 |
| Ctrl+Down Arrow | Move Line Down | 光标所在行下移一行 | 如中文 Down Arrow即鍵盤上的下箭頭 |
| Ctrl+Shift+D | Duplicate Lines | 重复添加光标所在行 | 如中文 |
| Ctrl+Shift+K | Delete Line | 删除光标所在行 | 如中文 |
| Ctrl+J | Join Lines | 加入行 | 测试效果为光标所在行的下一行追加到光标所在行后面 |

#### Columns 列
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Alt+Shift+Left Arrow | Move Selection Left | 光标所在位置向左选择一个单词/一句话 | 英文每个单词都会空一格，所以选中的是一个单词，而中文，如果一句话之中不存在数字、英文单词、英文特殊符号，那么选中的会是整句话 Left Arrow即鍵盤上的上箭頭 |
| Alt+Shift+Right Arrow | Move Selection Right | 光标所在位置向右选择一个单词/一句话 | 如上 Right Arrow即鍵盤上的上箭頭 |
| Shift+Left Arrow | Move Selection Left | 光标所在位置向左选择一个字符 | 英文选择一个字母，中文一个汉字 |
| Shift+Right Arrow | Move Selection Right | 光标所在位置向右选择一个字符 | 如上 |

#### Text 文本
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Upper Case | 大写 | 光标所在单词或选中的单词变成大写 |
|  | Lower Case | 小写 | 光标所在单词或选中的单词变成小写 |
| Ctrl+Delete | Delete to End of Word | 删除光标所在位置到词尾结束部分 | 英文删除选择一个单词的词尾，中文删除选择直到段落结束，或遇到数字、英文单词、英文特殊符号 |
|  | Delete to Previous Word Boundary | 删除光标所在位置到词头开始部分 | 英文删除选择一个单词的词头，中文删除选择直到段落开头，或遇到数字、英文单词、英文特殊符号 |
|  | Delete to Next Word Boundary | 删除光标所在位置到词尾结束部分 | 英文删除选择一个单词的词尾，中文删除选择直到段落结束，或遇到数字、英文单词、英文特殊符号 |
| Ctrl+Shift+K | Delete Line | 删除光标所在行 | 如中文 |
|  | Transpose | 转换位置 | 光标所在左右的字符颠倒位置，或者选择的部分全部颠倒位置 |

#### Folding 折叠
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Alt+Ctrl+[ | Fold | 展开段落 | 展开代码块 |
| Alt+Ctrl+] | Unfold | 折叠段落 | 折叠代码块 |
| Alt+Ctrl+Shift+] | Unfold All | 展开所有折叠段落 | 展开所有折叠代码块 |
| Alt+Ctrl+Shift+[ | Fold All | 折叠所有段落 | 折叠所有可折叠的代码块 |
|  | Fold Level 1~9 | 折叠当前文档相应层级的代码块 | 如中文 |

#### Bookmark 书签
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+F2 | View All | 查看所有书签【切换跳到书签位置】 | 可以给文档不同位置设置不同书签，然后这里都可以看到该文档所设置的所有标签 |
| Alt+Ctrl+F2 | Toggle Bookmark | 是否在光标处设置标签 | 通过此操作设置书签 |
| F2 | Jump to Next Bookmark | 跳到下一个标签位置 | 如中文 |
| Shift+F2 | Jump to Previour Bookmark | 跳到上一个标签位置 | 如中文 |

## View —— 视图
### 针对编辑器操作
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| F11 | Toggle Full Screen | 切换全屏模式 | 如中文 |
|  | Toggle Menu Bar | 切换菜单栏 | 此操作可隐藏菜单栏，按`alt`可暂时显示菜单栏，当编辑时，其会再次隐藏，若想一直显示， 则需再次执行此操作，或为此操作设置快捷键 |

#### pane 分屏
具体分屏操作，可看本教程[初识Atom——分屏][3]

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Split Up | 向上分屏 | 如中文 |
|  | Split Down | 向下分屏 | 如中文 |
|  | Split Left | 向左分屏 | 如中文 |
|  | Split Right | 向右分屏 | 如中文 |
|  | Focus Next Pane | 焦点聚焦于下一个分屏窗口 | 如中文 不分前后左右，只分先后顺序 |
|  | Focus Previous Pane | 焦点聚焦于前一个分屏窗口 | 如中文 不分前后左右，只分先后顺序 |
|  | Focus Pane Above | 焦点聚焦于上面的分屏窗口 | 如中文 |
|  | Focus Pane Below | 焦点聚焦于下面的分屏窗口 | 如中文 |
|  | Focus Pane On Left | 焦点聚焦于左面分屏窗口 | 如中文 有上下分屏的，聚焦上面的分屏 |
|  | Focus Pane On right | 焦点聚焦于右面分屏窗口 | 如中文 有上下分屏的，聚焦上面的分屏 |
|  | Close Pane | 关闭当前分屏窗口 | 如中文 |

#### Developer 开发人员
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Open In Dev Mode... | 在Dev分支上打开 | git托管项目操作，可将项目以dev分支在一个新窗口打开 |
|  | Reload Window | 重新加载窗口 | 重新打开一次编辑器 |
|  | Run Package Specs | 让包执行特定模式 | 未测试出具体用途 |
|  | Toggle Developer Tools | 显示/隐藏开发者工具 | 如中文(此编辑器的强大之处~!) |

***

### 针对字体操作
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+Shift+= | Increase Font Size | 放大编辑窗口字体字号 | 如中文 |
| Ctrl+Shift+- | Decrease Font Size | 缩小编辑窗口字体字号 | 如中文 |
| Ctrl+0 | Reset Font Size | 重置字体大小 | 如中文 |

### 其他分类
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Toggle Soft Wrap | 切换换行模式 | 编辑内容超过窗口宽度是否换行（即是否出现横向滚动条） |
| Ctrl+Shift+P | Toggle Command Palette | 显示/隐藏命令窗口 | 此操作可打开命令面板，包含此编辑器的所有命令操作，还可进行搜索命令操作，从命令列表内，可看到各命令的快捷键设置 |
| Ctrl+\ | Toggle Tree View | 切换目录树显隐状态 | 显示/隐藏目录树（执行此操作显示目录树时，会默认目录树为当前窗口，即聚焦目录树） |

## Selection —— 选择
### 添加选择
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Atl+Ctrl+Up Arrow | Add Selection Above | 选择部分追加到其上一行 | 选择光标所在行的任意位置的一段字符段，该操作可将其上一行相同字符数且该字符段的起始位置与光标所在行被选中的字符段的起始位距离该行的起始位置拥有相同的字符数 |
| Atl+Ctrl+Down Arrow | Add Selection Below | 选择部分追加到其下一行 | 同上 |
|  | Split into Lines | 分成行 | 未测试出具体用途 |
| Esc | Single Selection | 选择单行 | 未测试出具体用途 |

**解释一下此段两个选择：**
* `Add Selection Above`和`Add Selection Below`一个向上追加选择，一个向下追加选择
* 如不做选区，则追加选择的会是整行，其效果等同于先选择整行，然后追加选择上面一整行
* 做了选区，选区包含两项数据：**选区的字符数**、**选区起始位置到该行行首之间的字符数**
* 追加的行，其选区的字符数永远与用户选择的选区字符数相等，如遇到某行字符数少于选区字符数，则自动跳过该行，并继续寻找字符数相等的行
* 追加的行，行首到选区起始位置字符数如达不到，用户选择行的行首到选区起始位置的字符数，则自动跳过该行，并继续寻找行首到选区起始位置字符数相等的行
* 当然 **这两项数据必须同时成立，才会被选择，即如果只满足其中的一条，那么该行仍然会被跳过**
* 这里说字符数，在编辑器里其实应该是列,一个英文字母算一列，一个汉字也算一列

### 部分全选
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+Shift+Home | Select to Top | 选定从光标所在位置到顶部的所有内容 | 全选功能的分拆 |
| Ctrl+Shift+End | Select to Bottom | 选定从光标所在位置到底部的所有内容 | 全选功能的分拆 |

### 行内选择
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+L | Select Line | 选择行 | 全选光标所在行 |
|  | Select Word | 选择单词 | 如中文（选择中文时，选区遇到数字、英文单词、英文特殊符号才会截止） |
| Ctrl+Shift+Left Arrow | Select to Beginning of Word | 选择光标处到词头 | 如中文 |
|  | Select to Beginning of Line | 选择光标处到行首 | 如中文 |
| Shift+Home | Select to First character of Line | 选择光标处到行的第一个字符 | 测试效果同上一个到行首 |
| Ctrl+Shift+Right Arrow | Select to End of Word | 选择光标处到词尾 | 如中文 |
| Shift+End | Select to End of Line | 选择光标处到行尾 | 如中文 |
| Atl+Ctrl+M | Select Inside brackets | 选定括号内内容 | 括号需是英文的，小、中、大括号都可以，也可以是选定一个HTML标签的开始与结束之间的所有内容（包括标签开头加的类、ID等） |

## Find —— 查找
### 针对当前文件
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+F | Find in Buffer | 从缓冲区找 | 即从当前编辑文件中查找 |
| Alt+Ctrl+F | Replace in Buffer | 从缓冲区中查询替换 | 替换查找的内容（配合`Ctrl+F`使用） |
| Ctrl+D | Select Next | 查询及选定文件内下一个与用户选择相同的内容 | 如中文 |
| Alt+F3 | Select All | 查询及选定文件内所有与用户选择相同的内容 | 如中文 |
|  | Toggle Find in Buffer | 显示/隐藏查询窗口 | `Ctrl+F`之后，可通过按`Esc`来关闭查找窗口，也可通过此命令来关闭窗口，可为此命令添加快捷键，一键显隐查询窗口 |

### 针对项目
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+Shift+F | Find in Porject | 从工作目录查询 | 此命令需要聚焦目录树，可同时查找/替换该项目内所有用户要查找/替换的内容 |
| Alt+Ctrl+F | Toggle Find in Porject | 显示/隐藏工作目录查询窗口 | 如中文 |

### 针对查找对象
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+F | Find Next | 查找选定内容的下一个 | 匹配从选定内容之后开始的下一个相同内容 |
| Alt+Ctrl+F | Find Previous | 查找选定内容的上一个 | 匹配从选定内容之前开始的上一个相同内容 |
| Ctrl+D | Replace Next | 替换下一个 | 配合查询使用，为单个替换查询到的相同内容 |
| Alt+F3 | Replace All | 替换全部 | 根据查找方式，替换全部与查找相同的内容 |

### 针对历史
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Clear History | 清除历史 | 未测试出具体用途 |

### 针对编辑文本
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+B | Find Buffer | 查询缓冲区 | 查找在缓存区打开的所有文件，即编辑窗口内打开的所有文件 |
| Ctrl+P | Find File | 查询且打开文件 | 全局搜索并打开文件，即在该项目下搜索某个文件并打开 |
| Ctrl+Shift+B | Find Modifiled File | 查询编辑过的文件 | 即查询此次打开该编辑器，所有被编辑过/改动过的文件 |

## Packages —— 包
此处为用户为自己的Atom安装的所有插件包命令显示的地方，Atom安装后，会自身集成一些编辑器常用的插件包，用户如果想进行扩展，只需在Atom官网或github搜索安装即可。<br />
这里先简单介绍Atom集成的这些插件包：
### Bracket Matcher —— 括号匹配
* 就是会自动匹配`{}`,`[]`,`()`,`""`,以及反引号` `` `的结束标签。
* 光标在其中一个标签前后时，会同时将开始及结束标签都加一个下划线来高亮显示，这个作用也同时适用于XML和HTML标签

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+M | Go To Matching Bracket | 将游标移动到对应的方括号 | 即光标若在一对括号的一方，此操作会将光标移动到这一对括号的另一方(对HTML标签同样适用) |
| Alt+Ctrl+M | Select Inside Brackets | 选择标签内的内容 | 此命令在本文档`selection`章节的[行内选择](#行内选择)也有介绍 |
| Ctrl+] | Remove Brackets From Selection | 移除选区内的括号 | 只能移除英文各种括号且选区开始与结束是括号的开始与结束，选中后执行此操作，可将括号删除（此快捷键与Edit-Lines-Indent的快捷键冲突，这里不起作用，可另行设置） |
| Alt+Ctrl+Period | Close Current Tag | 关闭当前标签 | HTML标签的结束标签可通过此操作补全(`Period`即英文句号键) |
| Alt+Ctrl+Backspace | Remove Matching Brackets | 移除匹配的括号 | 选择英文括号的一边，执行此操作可将一对括号直接删除(不适用与HTML,`Backspace`即删除键) |

### Command Palette —— 命令面板
此项在`View视图-其他分类`中已讲到，此编辑器所有命令的列表

### Dev Live Reload —— 实时加载dev分支
此项为git项目插件，与本文档的`View-Developer-Open In Dev Mode...`一样，同属于git项目dev分支的操作。

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Alt+shift+Ctrl+R | Reload All Styles | 重新加载所有样式 | 如中文 |

### Git Diff —— 检索差异
此项为git托管项目的一个命令，当前工作目录项目和上次提交在这个命令下可发现哪些文件被修改了

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Move to Next Diff | 移动到下一个差异之处 | 如中文 |
|  | Move to Previous Diff | 移动aa到上一个差异之处 | 如中文 |
|  | Toggle Diff List | 显隐差异列表 | 如中文 |

### Keybinding Resolver —— 密钥绑定解析器
此包帮助用户理解执行了哪个快捷键，显示该窗口后，当你执行了一个快捷键后，窗口内会显示出此电脑定义了该快捷键的所有文件，可看出执行在了哪里,或者未执行的原因。

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Toggle | 显示/隐藏秘钥绑定解析器 | 直观显示快捷键命令执行情况 |

![][4]

> 解释此解析器的组成部分：
* 快捷键 —— 即此窗口头部会显示用户执行的快捷键
* 执行结果 —— 执行了命令的会高亮显示且信息前方为一个对勾符号，反之则为一个叉号。
* 命令名称 —— 即执行此命令的名称，改图为我执行了一次键盘上的删除键
* 执行部位 —— 即命令起效的地方，此处为文档的内部，body
* 命令定义的文件路径 —— 即定义了该快捷键命令的文件路径

**如果匹配到多个快捷键，Atom会根据选择器的特性以及他们被加载的顺序来决定执行哪个快捷键。命令未执行的两种情况（前提有这个快捷键命令）：**

1. 快捷键并没有在选择器定义的上下文中使用。例如，在目录树下有一个快捷键命令`a`，其意为添加一个新的文件，但此命令只能在焦点在目录树上时才能起作用，即在其他窗口，如编辑窗口直接键入`a`是不能触发该命令的。
2. 有另一个快捷键有更高的优先级。通常为安装包与现有的快捷键起冲突了，如果这个包的快捷键具有更高的特异性的选择器，或者更晚被加载，它就会覆盖现有的快捷键。

> Atom会首先加载核心功能的快捷键，之后才是用户定义的快捷键，当然想要解决快捷键冲突，可以编辑`File-Keymap...`来删除及重定义快捷键。

### Markdown Preview —— Markdown预览
Atom同样能支持Markdown语法编译，此插件包就是能让用户在编辑器中预览自己编写的markdown文档。

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+Shift+M | Toggle Preview | 显示/隐藏markdown文档预览窗口 | 如中文(快捷键很有可能会冲突) |

![][5]

用户可以在Atom中随心所欲的编写markdwon文档，并可通过此命令来实时预览效果~！

### Open On GitHub —— 在GitHub上打开
做为GitHub团队开发的编辑器当然要支持GitHub上打开啦~，当然项目必须已经push到了github上。

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Blame | Git命令显示提交信息 | 在此处的作用为在浏览器里打开文件的提交信息，通过此命令打开的文件，会在浏览器里逐行显示，并显示commi号，提交者，最早提交日期以及提交时的备注 |
|  | Branch Compare | 分支比较 | 比较两个分支的不同 |
|  | Copy URL | 复制链接 | 复制该项目在GitHub上的链接地址 |
|  | File | 在浏览器打开当前文件 | 如中文 |
|  | File on Master | 在Master分支打开当前文件 | 如中文 |
|  | History | 在浏览器里打开该项目的历史提交记录 | 如中文 |
|  | Issues | 问题 | 打开该项目在GitHub上的问题列表页面 |
|  | Repository | 存储库 | 打开该项目在GitHub上的版本库 |

### Package Generator —— 程序包生成程序

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Generator Atom Package | 生成Atom包 | 用户可以自己创建包， |
|  | Generator Atom Syntax Theme | 生成Atom语法主题 | 同样也可以自己创建语法主题 |

> 用户可以在Atom上发布自己的Package以及Syntax Theme,在这里可支持生成包

### Settings View —— 设置中心视图
即为菜单栏`File-Settings`

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+F1 | Open | 打开设置中心 | 如中文 |
|  | Show Keybindings | 显示快捷键界面 | 如中文 |
|  | Install Packages/Themes | 打开安装包/主题界面 | 如中文 |
|  | Update Packages/Themes | 打开更新包/主题界面 | 如中文 |
|  | Manage Packages | 管理包 | 打开包管理界面 |
|  | Manage Themes | 包里主题 | 打开主题管理界面 |

> 这里我们需要注意一点，在前文[2. Settings —— 设置中心](#2. Settings —— 设置中心)中提到打开设置中心快捷键是`Ctrl+,`,那么试过的都该知道，这个快捷键是不起作用的，这里就是[Keybinding Resolver —— 密钥绑定解析器](#Keybinding Resolver —— 密钥绑定解析器)讲到的快捷键冲突问题，真正其作用的是此处`Settings View`插件包设置的快捷键`Ctrl+F1`。

### Snippets —— 代码块
这里Atom本身集成的这个代码块，主要偏向于CoffeeScript的代码块，在GitHub上搜索`Snippets`,你会找到很多类似的代码块，且都有标注注重的语言，以及有多少人`fork`,`star`,当然你也可以在Atom官网搜索该包，更可以直接在此编辑器设置中心内的包管理里搜索相关包。

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Expand | 扩展 | 未测试出具体效果 |
| Tab | Next Stop | 代码块导入命令 | 代码块简写输入后，执行此命令，可在页面导入设置好的整块代码块 |
| Shift+Tab | Previous Stop | 未知 | 未测出具体效果 |
| Alt+Shift+S | Available | 打开可用代码块列表 | 即所有该插件有的相应语言的所有代码块简写命令列表 |

![][6]

> 这里Atom集成了很多语言的代码块，包括HTML、markdown等，可以通过`Alt+Shift+S`打开命令列表查看当前文件格式下的语言代码块

### Spell Check —— 拼写检查
打开或者关闭代码拼写正误检查，默认开启状态。

### Styleguide —— 样式指南

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+Shift+G | show | 打开样式指南 | 里面有该编辑器、字体颜色、标签代码着色、图标等的设置 |

### Symbols —— 标签符号表

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+R | File Symbols | 打开当前文件的标题列表 | 此命令可搜索出当前文档的标题，并形成列表，可点击直接跳到该位置 |
| Ctrl+Shift+R | Project Symbols | 打开项目文件列表 | 此处未测试具体效果 |

### Timecop —— 加载时间
打开该编辑器运行、缓存、插件包等加载时间的页面。

### Tree View —— 树视图
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Alt+\ | focus | 聚焦到树视图 | 即将焦点切换到项目目录树上 |
| Ctrl+\ | Toggle | 显示/隐藏树视图 | 打开/关闭项目目录树视图（同时有聚焦到目录树的作用） |
| Ctrl+Shift+\ | Reveal Active File | 显示活跃的文件 | 即将焦点聚焦在刚刚编辑的文件上（若编辑的文件在文件夹内未展开，则此命令为展开文件夹） |
|  | Toggle Tree Side | 目录树显示位置 | 即将目录树显示在编辑器的左侧/右侧 |

### Whitespace —— 空格
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Remove Trailing Whitespace | 删除尾随空格 | 如中文 |
|  | Convert Tabs to Spaces | 将制表符转换为空格 | 如中文 |
|  | Convert Spaces to Tabs | 将空格转换为制表符 | 如中文 |

## Help——帮助
### 开发团队
| 英文 | 中文 |
| :----- | :---- |
| View Terms of Use | github服务团队 |
| View License | 浏览许可证 |
| Version * | 用户安装版本 |
| Check for Update | 检查更新 |

### 使用帮助
| 英文 | 中文 |
| :----- | :---- |
| Documentation | Atom使用文档(英文版飞行手册) |
| Frequently Asked Questions | FAQ |

### Atom 社区
| 英文 | 中文 |
| :----- | :---- |
| Community Discussions | Atom社区讨论 |
| Report Issue | 报告问题 |
| Search Issue | 搜索问题 |

### 关于 Atom
| 英文 | 中文 |
| :----- | :---- |
| About Atom | 关于 Atom |

### 欢迎指南
| 英文 | 中文 |
| :----- | :---- |
| Welcome Guide | github服务团队 |

***

在这里只是对菜单栏的每一项做个简单介绍以及翻译，具体有些比较常用，或者这里没解释清楚的，后续会有相关文档，敬请关注~！

[1]:https://github.com/kaivin/atom/raw/master/images/interface/welcome.png "欢迎界面"
[2]:/settings.md "设置"
[3]:/pane.md "分屏操作"
[4]:https://github.com/kaivin/atom/raw/master/images/interface/keybinding.png "快捷键操作"
[5]:https://github.com/kaivin/atom/raw/master/images/interface/markdown.png "markdown预览"
[6]:https://github.com/kaivin/atom/raw/master/images/interface/snippets.png "代码块"
