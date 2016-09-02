# 为什么选择使用Atom
这里就不在去讨论哪个IDE更好的问题了，仁者见仁智者见智的事儿，在使用了git以及github之后，关注到了这个团队出的这款IDE，口号很响亮：“21世纪的黑客编辑器”，我只说说我为什么选择这款IDE：

* github团队研发，本着技术要用就用一整套的原则~，这一点让我对其有了一点倾向性。
* 开源，这一点对有点强迫症的我来说，就更友好了，本着只用最新版的原则~,多加一点倾向性。
* 可定制，这款IDE本身除了集成了一些IDE必备的插件外，想用什么其他插件，都可以根据需求去下载添加，其背靠github团队，有着强大的实力后盾。

我的IDE变迁史：DW-->WS(Webstorm)-->PS(PHPstorm)-->Atom

# 安装
那么既然选择了这款IDE，接下来就是安装了。打开Atom[官方首页][1]

![][2]

网页会自动判断你的操作系统,给出其对应的下载按钮。<br />
比如这里的windows系统（**本教程以后章节均为windows系统**）,其他系统这里的按钮是不一样的，具体根据自己的系统打开页面就可发现。点击下载按钮即可。<br />
如果要下载其他系统的安装包,点击[Other platforms][3]链接即可,这里打开的即是atom在github开源库，选择标签`tags`,可在其发布的版本中，任意选择下载版本压缩包。

![][4]

## MAC
如果是MAC系统，解压下载的zip安装包，将解压的Atom应用拖到应用目录下<br />
或者通过Homebrew Cask安装：
```
brew cask install atom
```
## windows
windows系统只需运行安装包即可，如果是在github上，下载的版本压缩包，解压即可使用。

## Linux
如果是基于Debian的发行版,执行命令:
```
sudo dpkg -i atom-amd64.deb
```
如果是RedHat,则执行:
```
rpm -i atom.x86_64.rpm
```

# 安装完成
安装完成双击快捷方式，就进入了Atom界面了。

> ### Tips
> 需要注意的是，安装完成后会默认安装apm，而apm则是atom的核心package必备命令行，命令行中操作下载插件都需要用到apm,而检查apm是否安装完成则可以通过命令行来测试：
> 按`cmd+r`输入`cmd`运行cmd 并在cmd内输入`apm -v`如出现版本信息，则表示已安装成功。
> 如提示不是内部命令，则代表未安装成功或者环境变量未配置。apm会安装在你电脑当前用户的一下路径内：
> ```C:\Users\Administrator\AppData\Local\atom\app-1.10.0\resources\app\apm\bin```
> 如没有，则表示安装出错，因为此命令已经被内置到atom安装包内，可在官网重新下载安装，当然以上路径是本人的安装路径，其中`Administrator`以及`app-1.10.0`是根据你自己电脑用户以及你所安装版本而变的。
> 如存在该路径，还是提示不是内部命令，则可能是环境变量未配置。
> 环境变量的配置，右键我的电脑->属性：

![][5]

如上图所示，如果在环境变量中找到apm路径，查看路径是否正确，如没有，则在系统变量中新建变量，命名`app_path`，变量值则填写你的安装路径，一般均为上述默认路径，只在电脑当前用户以及版本这两个地方有所改动。

好了，准备工作已经完成，让我们开始atom编辑之旅吧！~

[1]:https://atom.io/ "Atom官网"
[2]:https://github.com/kaivin/atom/raw/master/images/install/download.png ""
[3]:https://github.com/atom/atom/releases/ "发布版本"
[4]:https://github.com/kaivin/atom/raw/master/images/install/github.png ""
[5]:https://github.com/kaivin/atom/raw/master/images/install/path.png ""
