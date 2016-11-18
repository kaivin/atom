# 初识Atom(9) —— package安装方法以及apm使用方法

Atom安装可以有一下三种方法：

## Atom编辑器中直接下载

`settings -> install`中搜索相应的package,直接在Atom中`install`，有些插件在这里可能搜到但是显示不出来，需要下面的方法。

## github或Atom官网下载压缩包

到[github][7]或者[Atom官网][8]上搜索相应的package,在浏览器中下载最新版本，然后放到安装atom目录的`packages`文件夹内,重新打开编辑器，就可以在packages中找到安装的插件。

在[Atom官网][8]`package`栏目中搜索插件后如下图：

![][9]

从这里可以看到该插件的下载量及版本，也可以点击`Repo`进入该插件在github上的首页，点击`Versions`则直接进入github上该插件的版本下载界面，下载最新版本的压缩包解压到 `~/.atom/packages` (即 `C:/用户/当前用户名/.atom/packages/`)文件夹内,然后通过命令行 `cd` 到该 `package`文件夹，再直接输入 `apm install` 进行安装，当后面显示`done`时，就证明已经安装成功。

在[github][7]直接搜索：

![][10]

点击进入插件如下：

![][11]

这里只要点击`releases`即可进入版本压缩包下载页面。下载最新版本的压缩包解压到 `~/.atom/packages` (即 `C:/用户/当前用户名/.atom/packages/`)文件夹内,然后通过命令行 `cd` 到该 `package`文件夹，再直接输入 `apm install` 进行安装，当后面显示`done`时，就证明已经安装成功。


## 使用`apm`命令安装

在本教程第一章[初识Atom(1) —— 安装Atom][1]中已讲到apm的配置问题，这里假设`apm`已能正常运行的情况下,`Win+R`运行输入`cmd`打开命令面板，我们可以通过输入`apm`回车，来查看所有`apm`的命令:

![][2]

如果一个包，不知道具体的名字，可通过命令模糊搜索，比如`apm search color`,搜索与颜色相关的插件包：

![][3]

它会列出所有与颜色有关的插件，且显示搜索与`color`有关的结果有25个，从这些中找到自己想要安装的插件，比如我想安装的是`color-picker`插件（一个非常强大的拾色器），就可以从这里找到插件的名字

如果想要知道这个插件的详细信息，可以通过`apm home color-picker`命令来查看，该命令会用默认浏览器打开该插件的首页，确认是自己想要安装的插件后，输入命令`apm install color-picker`

![][4]

可以从安装中看到，包的安装路径，也就是编辑器的安装目录中`packages`文件夹，当后面显示`done`时，就证明已经安装成功。

安装成功后，命令行中输入`apm list`可以查看编辑器已经安装的包：

![][5]

上面出现的是编辑器自带的包，下面`Community Packages <2>`就是用户自己安装的包。

使用命令行安装完插件包后，我们需要重新加载一下Atom编辑器，`Alt+Ctrl+R`重新加载编辑器。然后就可以在`settings -> packages`界面中的`Community Packages`列表中看到已经安装了`color-picker`插件包。

那么如果用户不需要某个已经安装的包，也可以通过命令行来操作：`apm uninstall color-picker`,与安装一样，卸载完成后，其后面也会显示`done`：

![][6]

那么剩下的就是随心所欲的去订制自己偏好的编辑器吧~！

> ps:有时可能会因为墙的原因而无法下载，或者速度超慢，这是让人无法忍受的~，所以作为前端开发还是要学会翻墙的~！

***

[1]:/install.md "安装Atom"
[2]:https://github.com/kaivin/atom/raw/master/images/package/apm1.png "apm命令"
[3]:https://github.com/kaivin/atom/raw/master/images/package/apm2.png "apm命令"
[4]:https://github.com/kaivin/atom/raw/master/images/package/apm3.png "apm命令"
[5]:https://github.com/kaivin/atom/raw/master/images/package/apm4.png "apm命令"
[6]:https://github.com/kaivin/atom/raw/master/images/package/apm5.png "apm命令"
[7]:https://github.com/ "github官网"
[8]:https://atom.io/packages/ "Atom官网"
[9]:https://github.com/kaivin/atom/raw/master/images/package/atom.png "atom插件界面"
[10]:https://github.com/kaivin/atom/raw/master/images/package/github1.png "github插件界面"
[11]:https://github.com/kaivin/atom/raw/master/images/package/github2.png "github插件界面"
