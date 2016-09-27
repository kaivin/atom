# 初识Atom(8) —— 工作区

上一章已经提前说到了Atom的分屏操作，对于需要多种文件同时编辑的工作来说，分屏操作提供了非常人性化的便捷之法。而本章，将细化说到在编辑文件中，用到的各种操作。

# 目录
* [移动跳转](#移动跳转)
* [文本选择](#文本选择)
* [编辑删除](#编辑删除)
* [查找替换](#查找替换)
* [代码片段](#代码片段)
* [自动补全](#自动补全)
* [折叠代码](#折叠代码)
* [语法格式](#语法格式)

本章内容大部分都在[初识Atom(2) —— 菜单栏][1]一章中，`编辑`、`选择`、`查找`区块内有具体的命令讲解。这里算是做一次集中复习吧，也同时说一些，在菜单栏中未提到一些命令操作。

## 移动跳转

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+G | Go to Line | 跳转到某行 | 可跳转到行，也可跳转到某行的某列位置，语法row:columns。例：20:30——>20行30列 |
| Ctrl+Up Arrow | Move Line Up | 光标所在行上移一行 | 如中文 Up Arrow即鍵盤上的上箭頭 |
| Ctrl+Down Arrow | Move Line Down | 光标所在行下移一行 | 如中文 Down Arrow即鍵盤上的下箭頭 |
| Alt+Left Arrow |  | 光标向左移一个单词 | 如中文 |
| Alt+right Arrow |  | 光标向右移一个单词 | 如中文 |
| Alt+B |  | 光标向左移一个单词 | 如中文 |
| Alt+F |  | 光标向右移一个单词 | 如中文 |
| Ctrl+M |  | 相应括号之间，html tag之间等跳转 | 光标在一个标签的开始与结束处的跳转 |
| Ctrl+R |  | 在当前文档的符号间跳转 | 符号是指Symbols,包括代码中的函数名,变量名，标签名等  |
| Ctrl+Shift+R |  | 在该项目内搜索并跳转到符号 | 需要tags文件的支持 |

需要说明的是`Ctrl+G`跳转到某行：

![][2]

使用`Ctrl+G`弹出以上窗口，输入 行:列 后回车就可将光标移动到指定位置，也可直接填入要跳转的行，直接跳转到行的起始位置。

还有一点符号间的跳转`Ctrl+R`,键入命令，弹出符号列表，针对不同文件，会有不同的符号列表，如markdown文件的标题列表，HTML文件的标签列表等等，也可同过搜索来跳转到目的地行。

`Ctrl+Shift+R`首先，你需要确保你的项目中生成了tags（或者TAGS）文件。通过安装ctags，并且从命令行中，在你的项目根目录下运行ctags -R src/这样的命令，来生成文件。

你可以通过在你的主目录下生成.ctags文件（~/.ctags），来自定义tags如何生成。

符号浏览功能在atom/symbols-view包中实现。

### 书签跳转

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+F2 | View All | 查看所有书签【切换跳到书签位置】 | 可以给文档不同位置设置不同书签，然后这里都可以看到该文档所设置的所有标签 |
| Alt+Ctrl+F2 | Toggle Bookmark | 是否在光标处设置标签 | 通过此操作设置书签 |
| F2 | Jump to Next Bookmark | 跳到下一个标签位置 | 如中文 |
| Shift+F2 | Jump to Previour Bookmark | 跳到上一个标签位置 | 如中文 |

![][3]

使用`Alt+Ctrl+F2`在光标处创建书签，创建书签后，光标所在行行首位置会多出一个小图标，以示创建成功，通过`Ctrl+F2`查看书签列表，点击列表中的书签即可跳转到书签所在位置。

## 文本选择

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Alt+Shift+Left Arrow | Move Selection Left | 光标所在位置向左选择一个单词/一句话 | 英文每个单词都会空一格，所以选中的是一个单词，而中文，如果一句话之中不存在数字、英文单词、英文特殊符号，那么选中的会是整句话 Left Arrow即鍵盤上的上箭頭 |
| Alt+Shift+Right Arrow | Move Selection Right | 光标所在位置向右选择一个单词/一句话 | 如上 Right Arrow即鍵盤上的上箭頭 |
| Shift+Left Arrow | Move Selection Left | 光标所在位置向左选择一个字符 | 英文选择一个字母，中文一个汉字 |
| Shift+Right Arrow | Move Selection Right | 光标所在位置向右选择一个字符 | 如上 |

下面把在[初识Atom(2) —— 菜单栏][1]一章`选择`中，提到的命令再列出来熟悉一下：

### 添加选择
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Atl+Ctrl+Up Arrow | Add Selection Above | 选区追加到其上一行 | 选择光标所在行的任意位置的一段字符段，该操作可将其上一行相同字符数且该字符段的起始位置与光标所在行被选中的字符段的起始位距离该行的起始位置拥有相同的字符数 |
| Atl+Ctrl+Down Arrow | Add Selection Below | 选区追加到其下一行 | 同上 |
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

### 其他选择
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+Shift+D |  | 复制当前行并添加到其下一行 | 如中文 |
| Ctrl+click |  | 添加新光标 | 神一样的用法，通过该命令可同时为多行设定光标，同时输入内容 `click`为点击鼠标左键 |
| Ctrl+D |  | 选取文档中和当前单词相同的下一处 | 如中文 |

## 编辑删除

### 单项

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+/ | Toggle Comments | 添加注释 | 可根据文件格式智能选择何种注释符 |
| Alt+Ctrl+Q | Reflow Selection | 浮动选择区域 | 测试效果为光标所在的行追加到其上一行的后面 |
| Ctrl+Shift+U | Select Encoding | 选择文件编码格式 | 如中文 |
| Ctrl+Shift+L | Select Grammar | 选择语法格式 | 给文件选择一种语言格式，也就是什么后缀的文件 |


### Lines 行

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+] | Indent | 缩进 | 光标所在行缩进，其效果如同`Tab`,区别在于光标在行的任何位置，此快捷键都是缩进此行，而非光标在哪里就从哪里缩进 |
| Ctrl+[ | Outdent | 回退缩进 | 撤销通过`Ctrl+]`产生的缩进 |
|  | Auto Indent | 自动缩进 | 无测试效果 |
| Ctrl+Up Arrow | Move Line Up | 光标所在行上移一行 | 如中文 Up Arrow即鍵盤上的上箭頭 |
| Ctrl+Down Arrow | Move Line Down | 光标所在行下移一行 | 如中文 Down Arrow即鍵盤上的下箭頭 |
| Ctrl+Shift+D | Duplicate Lines | 重复添加光标所在行 | 如中文 |
| Ctrl+Shift+K | Delete Line | 删除光标所在行 | 如中文 |
| Ctrl+J | Join Lines | 加入行 | 将下一行合并到当前行 |

### Columns 列

| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Alt+Shift+Left Arrow | Move Selection Left | 光标所在位置向左选择一个单词/一句话 | 英文每个单词都会空一格，所以选中的是一个单词，而中文，如果一句话之中不存在数字、英文单词、英文特殊符号，那么选中的会是整句话 Left Arrow即鍵盤上的上箭頭 |
| Alt+Shift+Right Arrow | Move Selection Right | 光标所在位置向右选择一个单词/一句话 | 如上 Right Arrow即鍵盤上的上箭頭 |
| Shift+Left Arrow | Move Selection Left | 光标所在位置向左选择一个字符 | 英文选择一个字母，中文一个汉字 |
| Shift+Right Arrow | Move Selection Right | 光标所在位置向右选择一个字符 | 如上 |

### Text 文本
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Upper Case | 大写 | 光标所在单词或选中的单词变成大写 |
|  | Lower Case | 小写 | 光标所在单词或选中的单词变成小写 |
| Ctrl+Delete | Delete to End of Word | 删除光标所在位置到词尾结束部分 | 英文删除选择一个单词的词尾，中文删除选择直到段落结束，或遇到数字、英文单词、英文特殊符号 |
|  | Delete to Previous Word Boundary | 删除光标所在位置到词头开始部分 | 英文删除选择一个单词的词头，中文删除选择直到段落开头，或遇到数字、英文单词、英文特殊符号 |
|  | Delete to Next Word Boundary | 删除光标所在位置到词尾结束部分 | 英文删除选择一个单词的词尾，中文删除选择直到段落结束，或遇到数字、英文单词、英文特殊符号 |
| Ctrl+Shift+K | Delete Line | 删除光标所在行 | 如中文 |
|  | Transpose | 转换位置 | 光标所在左右的字符颠倒位置，或者选择的部分全部颠倒位置 |
| Ctrl+Shift+Del |  | 删除光标处到单词尾 | 如中文 |

## 查找替换

### 针对当前文件
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+F | Find in Buffer | 从缓冲区找 | 即从当前编辑文件中查找 |
| Alt+Ctrl+F | Replace in Buffer | 从缓冲区中查询替换 | 替换查找的内容（配合`Ctrl+F`使用） |
| Ctrl+D | Select Next | 查询及选定文件内下一个与用户选择相同的内容 | 如中文 |
| Alt+F3 | Select All | 查询及选定文件内所有与用户选择相同的内容 | 如中文 |
|  | Toggle Find in Buffer | 显示/隐藏查询窗口 | `Ctrl+F`之后，可通过按`Esc`来关闭查找窗口，也可通过此命令来关闭窗口，可为此命令添加快捷键，一键显隐查询窗口 |

![][4]

### 针对项目
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+Shift+F | Find in Porject | 从工作目录查询 | 此命令需要聚焦目录树，可同时查找/替换该项目内所有用户要查找/替换的内容 |
|  | Toggle Find in Porject | 显示/隐藏工作目录查询窗口 | 如中文 |

![][5]

### 针对查找对象
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| F3 | Find Next | 查找选定内容的下一个 | 匹配从选定内容之后开始的下一个相同内容 |
| Shift+F3 | Find Previous | 查找选定内容的上一个 | 匹配从选定内容之前开始的上一个相同内容 |
|  | Replace Next | 替换下一个 | 配合查询使用，为单个替换查询到的相同内容 |
|  | Replace All | 替换全部 | 根据查找方式，替换全部与查找相同的内容 |

### 针对历史
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
|  | Clear History | 清除历史 | 未测试出具体用途 |

### 针对编辑文件
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Ctrl+B | Find Buffer | 查询缓冲区 | 查找在缓存区打开的所有文件，即编辑窗口内打开的所有文件 |
| Ctrl+P | Find File | 查询且打开文件 | 全局搜索并打开文件，即在该项目下搜索某个文件并打开 |
| Ctrl+Shift+B | Find Modifiled File | 查询编辑过的文件 | 即查询此次打开该编辑器，所有被编辑过/改动过的文件 |

## 代码片段
代码段是一个非常有效的工具，可以从一个快捷方式中快速生成常用的代码语法。

许多包自带他们自己的，具有特定模式的代码段。比如，提供了html语法高亮和语法的`language-html`包提供了许多代码段，来创建一些你想使用的不同HTML标签。如果你在Atom中创建一个新的HTML文件，你可以输入`html`然后按下`tab`，它会扩展为：

```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title></title>
    </head>
    <body>

    </body>
</html>
```
同时它会把光标放在`title`标签的中间，以便你立即开始填充这个标签。许多代码段具有多个焦点位置，你可以按下tab在他们之间切换 —— 比如，在这个HTML代码段之中，你填充完标题标签之后，可以按下`tab`键，然后光标就会移动到`body`标签之间。

要查看当前打开文件拥有的所有代码段，你可以按下`alt-shift-S`。

![][6]

这里是`markdown`的代码块的列表。用户可以直接通过输入`img`然后按下`tab`，那么会直接输出`![]()`,其他语言也是一样的道理，是不是很方便？~

插件中未提供，而平时又用到的比较多的一些代码块，用户可以非常便利的自己添加。

打开`file` -> `snippets...`，其文件与`keymap...`一样都是`.cson`后缀：

![][7]

这里就以该图中的示例来讲解：

```
 '.source.coffee':
   'Console log':
     'prefix': 'log'
     'body': 'console.log $1'
```

其所代表的意思：

```
 '选择范围':
   '描述':
     'prefix': '键入内容'
     'body': '输出内容'

```
安装Atom后，Atom自身集成了很多语言的模块包，可以在`settings` -> `packages`中找到，那么打开此例`coffee script`的语言包`language-coffee-script`

可以直接点击包名，浏览器中打开的为github上该包的路径，可以在这里看到该插件包的所有更新内容以及所有代码块。

当然，也可以直接点击`setting`，在编辑器中打开该插件包的设置界面。在这个界面的下方，会列出该插件包，包含的所有代码块的命令列表：

![][8]

![][9]

把示例与上图中代码块命令进行比对，可以发现：

* `描述`就是列表中的`Name`(这里可能有所改动，可以打开该包在github的`language-coffee-script.cson`文件查看)，描述可以是中文。
* `输出内容`就是列表中的`body`
* `键入内容`就是列表中的`Trigger`
* 也就是说`Trigger`和`perfix`代表的是一个内容，即触发命令提示语。
* 至于选择范围，可以看该包在github上的`snippets`文件夹下的`.cson`文件内的第一行，即为该语言的选择范围。当然也可以直接看编辑器中，该语言包的插件`setting`中的`scope`(上图红框中的部分)部分，并在前面加上一个`.`

接下来，我们就自己创建一个属于自己的代码块~ 比如，我想创建一个`dl-dt-dd`的代码块，还要给dl一个类，并且想以`ddd`为触发命令， 遵循以上模板：
```
'.text.html':
  'dl dt dd代码组':
    'prefix': 'ddd'
    'body': '<dl class="$1">\n\t<dt>$2</dt>\n\t<dd>$3</dd>\n</dl>$0'
```

`.text.html`选择范围可以查看Atom编辑器集成的`language-html`插件包中的`language-html/snippets/language-html.cson`该路径文件第一行即可。

`body`的输出内容里`/n`以及`/t`代表`新的一行`和`前进一个制表符`这样，输出的代码就是正确的格式，而`$0,$1,$2,$3`则为光标在`tab`切换时，可以以顺序切换到相应的地方，`$0`在`tab`切换完该代码块的所有位置后，会切换到这里，光标会首先在`$1`的位置，按`tab`切换后会到`$2`的位置，以此类推。`/t`可以多个`t`多一个`t`表示多缩进一个制表符。

`.text.html`为选择区，所有该选区内的代码块都写在这个选区下，如例中，`描述`缩进一个制表符，以及之后的`键入内容`、`输出内容`再在`描述`的基础上缩进一个制表符。

将以上代码写在`snippets.cson`文件内保存之后，这个代码块就已经创建完成了~ 打开一个html文件，输入`ddd`再按`tab`键，我想要的效果出现啦！：
```
<dl class="">
    <dt></dt>
    <dd></dd>
</dl>
```

当然了，代码块也允许你定义一个多行的代码块区别就是，多行的`body`后面的输出内容用 **3个双引号** -> `""" 输出内容 """`：
```
'.text.html':
  'dl dt dd代码组':
    'prefix': 'ddd'
    'body': """
        <dl class="$1">
            <dt>$2</dt>
            <dd>$3</dd>
        </dl>$0
    """
```
这样也能达到输出一样的效果~

## 自动补全
通常，自动补全工具会浏览当前打开的整个文档，寻找匹配你开始打出来的单词。

如果你想要更多选项，在设置面板的Autocomplete包中，你可以设置为在所有你打开的缓冲区中寻找字符串，而不仅仅是当前文件。

自动补全功能在atom/autocomplete包中实现。

在`settings` -> `packages`中，可以看到很多`autocomplete`开头的插件包，有`html`、`css`、`snippets`等，进入该插件可以看到具体图片演示，简单易懂。


## 折叠代码

当你把鼠标移到数字栏上，你就可以点击显示的箭头来折叠代码段。你也可以使用快捷键`Alt-Ctrl-[`和`Alt-Ctrl-]`来折叠和展开代码段。

![][10]

### Folding 折叠
| 快捷键 | 英文 | 中文 | 作用 |
| :----- | :---- | :----- | :----- |
| Alt+Ctrl+[ | Fold | 展开段落 | 展开代码块 |
| Alt+Ctrl+] | Unfold | 折叠段落 | 折叠代码块 |
| Alt+Ctrl+Shift+] | Unfold All | 展开所有折叠段落 | 展开所有折叠代码块 |
| Alt+Ctrl+Shift+[ | Fold All | 折叠所有段落 | 折叠所有可折叠的代码块 |
|  | Fold Level 1~9 | 折叠当前文档相应层级的代码块 | 如中文 |

## 语法格式

如果你加载了一个文件，Atom会做一些工作来试图识别出文件的类型。大部分情况，Atom通过查看文件的扩展名（.md通常为一个Markdown文件，等等）来完成。然而有时扩展名难以判断，它会检查内容来进行识别。

如果你加载了一个文件，并且Atom不能判断文件的语法，它会默认为纯文本（Plain Text），这是最简单的类型。如果它把文件默认为纯文本，或者弄错了文件类型，再或者由于一些原因你想修改文件的活动语法，你可以按下`ctrl-shift-L`下拉语法选择工具。

一旦你手动修改了一个文件的语法，Atom会记住它，直到你将语法设置回“自动检查”，或者手动选择一个不同的语法。

语法选择工具的功能在`atom/grammar-selector`包中实现。

![][11]

到此编辑器本身这一块就算全部讲完啦~，接下来就要为自己的编辑器按需加载插件包，实现定制性编辑器啦！


***
[1]:/menuBar.md "菜单栏"
[2]:https://github.com/kaivin/atom/raw/master/images/workspace/gotoline.png "跳转到某行"
[3]:https://github.com/kaivin/atom/raw/master/images/workspace/bookmark.png "书签"
[4]:https://github.com/kaivin/atom/raw/master/images/workspace/find1.png "文件内查找"
[5]:https://github.com/kaivin/atom/raw/master/images/workspace/find2.png "项目内查找"
[6]:https://github.com/kaivin/atom/raw/master/images/workspace/snippets.png "代码块"
[7]:https://github.com/kaivin/atom/raw/master/images/workspace/snippets1.png "代码块"
[8]:https://github.com/kaivin/atom/raw/master/images/workspace/snippets2.png "代码块"
[9]:https://github.com/kaivin/atom/raw/master/images/workspace/snippets3.png "代码块"
[10]:https://github.com/kaivin/atom/raw/master/images/workspace/zd.png "折叠"
[11]:https://github.com/kaivin/atom/raw/master/images/workspace/yf.png "语法选择"
