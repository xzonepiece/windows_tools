# windows_tools
Windows上的神器，改善Windows使用体验，提高Windows操作效率

## 最快搜索软件 - [Everything](http://www.voidtools.com)/[Listary](http://www.listary.com/)
Windows7的搜索实在是太慢了，而搜索对于我们来说，实在是太重要啦。我们经常需要在电脑上查找一些文件，或者要打开一些文件，尤其是对于我这种经常将文件乱放的人来说，搜索文件基本上是我每天都要做的事情。也行你会觉得应该将文件仔仔细细地整理好，不就可以少一些搜索吗，但是，搜索一个文件其实要比不停地打开文件夹快得多；而且，我们经常要面对一些琐碎的文件，这些文件根本就无法整理，即使整理了，你也会很快忘记。说了这么多废话，我就想告诉大家，搜索真的很重要，但是Windows7自带的搜索简直不能忍，不过，你现在可以不用担心啦，因为我们有Everything这款神器（安装包不到1MB），它的搜索甩Windows自带搜索好几条街，而且还**支持基本的搜索语法和强大的正则表达式**。
下面分享一些自己常用的搜索语法：
```
基本符号：|(或)、!(非)、*(匹配任意个任意字符)、?(匹配一个任意字符)
修饰符号：casecase(匹配大小写)、file(只匹配文件)、folder(只匹配文件夹)、path(匹配路径和文件名)、regex(正则表达式)
函数：datecreated:<date>(搜索特定创建日期的目标)、len:<length>（筛选出特定长度的目标名）、size:<size>（搜索特定大小的文件）
```
简单举例：比如我想从E盘“简书”文件夹下面搜索出这个月创建的图片，图片的格式为jpg,文件名中包含“工具”两个字，我们可以这样写：**E:\简书\*工具*.jpg datecreated:2016/3/1-today**!
>如果你想更深入的使用Everything的话，强烈建议学习正则表达式。

**Listary**也是一款强大的搜索工具，搜索速度比Everything相当，而且，Listary在搜索到文件之后，会直接打开文件或文件夹。不过，它不支持搜索语法和正则表达式，付费版才支持模糊搜索。但是，Listary又不仅仅是一款搜索工具，它还具有其他强大的功能，比如智能命令、最近文档、收藏文件（鼠标双击就可以访问这些功能），等等。
这两款工具，我都有安装，**如果是只是简单的搜索文件或文件夹，并且要打开它的话，我会使用Listary；如果是寻找某一个或一些特定的文件或文件夹，我会使用Everything**。
**使用这两款搜索工具还有个最大的前提，就是要好好地命名文件和文件夹，不然，你以后搜文件的时候也是搜不到你想要的。**
>如果你是一个整理狂魔的话，推荐你使用**文件管理神器Total Commander**,不过，因为颜值不符合我的要求，我用了一段时间就放弃了，但是，这个文件管理神器真心很强大，搜索文件、文件内容比较、同步文件夹、批量重命名文件、分割合并文件......只有你想不到的，没有它做不到的，即使有它自己做不到的，也可以使用第三方插件满足你的要求。
### Windows启动软件- [Wox](http://www.getwox.com/)

在上一篇文章中，我简单的介绍了快速启动软件[Launchy](http://launchy.net/)，它的确是一款优秀的启动软件，可是，作者已经好久没有更新，而且这款软件的可扩展性不是很好，直到我遇见了这款Windows专属的快速启动软件Wox。

Wox的设计初衷来源于Mac 上 的Alfred 和 Window 上的 Launchy，至于Alfred，我没有用过，只知道它是Mac上的效率神器，不知道Wox有没有做到在Windows上堪比Mac上的Alfred，但是，对于Launchy，我觉得Wox做的可能比它更好，因为Wox的可扩展实在太棒了，它支持C#和Python扩展，这对于我这种只会Python这一门高级语言的人来说，简直就是福音。

Wox目前的功能包括：

1. 搜索本机文件，其内置[everything](http://www.voidtools.com/)，搜索非常快，而且还支持拼音搜索程序，这对中文用户来说，实在太赞了（不亏为国人大牛，so sweet）；
2. web search功能，通过给某个网址设置关键字直接搜索，这个是系统自带的插件，launchy也有这个功能；
3. 可[定制主题](http://www.getwox.com/theme/builder)，这里的定制主题只能改变搜索框等的颜色和透明度等等，样式有点单薄，但是，原本的这个样式颜值也不差；
4. 可添加自定义[扩展](http://www.getwox.com/plugin)，几乎任何语言都可以用来编写 Wox 插件，最主要是C#和Python，官网上也有很多插件可供安装使用，比如，查单词、查快递、查剪贴板历史等等。

有一点需要注意的是，该软件仍应处于开发测试阶段，发行的版本仍存在一些bug问题，比如目前的[v1.3.67](https://github.com/Wox-launcher/Wox/releases)在使用python插件时，需要手动将wox.py文件拷贝到插件目录。

### 全局鼠标手势软件-[WGestures](http://www.yingdev.com/projects/wgestures)

不知道大家喜不喜欢使用鼠标手势软件，以前我不是很喜欢用，但是，自从使用猎豹浏览器（自带鼠标手势）之后，就开始喜欢上这种高效的操作方式（不过，我现在已经不怎么用猎豹浏览器了，现已成为谷歌Chrome浏览器中毒使用者，当然，这是题外话）。在习惯这种操作方式之后，我开始想在任何位置都可以使用这种方式，而不仅仅只局限于浏览器，所以就遇到了这款强大的免费的全局鼠标手势软件，它的功能真是无比强大。

WGestures的**Github项目主页**在[这里](https://github.com/yingDev/WGestures)，下面这张图介绍了它的复制粘贴功能。WGestures还可以使用手势来执行前进、后退、关闭窗口、最大化、最小化、打开网址、运行程序、执行快捷键等等实用的操作（我最喜欢窗口置顶、向上翻页、撤销关闭页面等各种手势），而且可以完全自定义。如果配合[Clover](http://cn.ejie.me/)使用，可以像操作浏览器那样操作资源管理器。

### Windows脚本语言-[AutoHotkey](https://autohotkey.com/)

可能一说到语言，就已经有人望而退步了，但是，作为只支持WIndows的脚本语言，AutoHotkey使用起来非常简单，几行简单的代码就能实现非常强大的功能。

至于AutoHotkey能做什么，我只能说，这完全取决于你的想象，但是，它最最主要的功能还是完成Windows中的一些常见操作，维基百科上对于它的解释是：**AutoHotkey**是面向普通电脑用户的自由开源的自动化软件，它让用户能够快捷或自动执行重复性任务。所以，最重要的一点是，它最主要的功能还是帮助大家自动执行重复性的工作，比如热键、热字串、重映射键盘、操作窗口、字符串处理等等这类的操作，但是，需要注意的是，AutoHotKey不比Python这种全能型的脚本语言，对于复杂的操作，应该把它当成桥梁，用来操作其他工具或语言，从而来满足我们的需求，比如，我之前通过Python和AutoHotkey完成了Markdown中的快速贴图，具体参见我的简书文章-[Markdown 最强最快贴图方法](http://www.jianshu.com/p/6fb3e2151f90)。

使用方法参见这篇[快速入门教程](http://ahkcn.sourceforge.net/docs/Tutorial.htm)，基本上就已经够用了；这篇[AutoHotkey学习指南](https://autohotkey.com/boards/viewtopic.php?f=29&t=1099)基本上罗列了从入门到精通的大部分学习资料，而且，网上现成的代码也是一抓一大把，比如，这篇博客上介绍的一些[AutoHotkey常用脚本](http://benq.im/2015/12/25/ahk/)，官网上也有专门的[中文论坛版面](https://autohotkey.com/boards/viewforum.php?f=26)。

## 资源管理器扩展 - [Clover](http://cn.ejie.me)
比起Windows资源管理管理已打开文件夹的方式，我更喜欢谷歌chrome浏览器管理已打开网页的方式-使用多标签页，通过点击不同的标签来查看不同的网页。Clover就是一款这样的工具软件，它可以为Windows资源管理器增加类似谷歌 Chrome 浏览器的多标签页功能。而且，它还具有浏览器的书签功能（收藏文件夹），重启时可以重新打开最后一次打开的标签页。

## 截图 - [FastStone Capture](http://www.portablesoft.org/faststone-capture/)
FastStone Capture是一款非常强大的截屏工具，支持活动窗口截图、矩形区域截图、手绘区域截图、整个屏幕截图、滚动窗口截图、固定区域截图等各种需求。其中，滚动窗口截图的功能超级强大，可以轻松制作出超长的截图。除了最基本的截图功能，它还可以编辑图片（裁切，标记等），拥有屏幕取色器、屏幕标尺、将图像转换为 PDF 文件、将截图发送到 PPT、Word、FTP等强大的功能，而且，它还支持录屏。

## 其他工具
- 翻译神器-[QTranslate](http://www.portablesoft.org/qtranslate-portable/)
- 窗口停靠神器-[Dockit](http://www.appinn.com/dockit-for-win/)
- 最美字体神器-[MacType](http://www.appinn.com/mactype/)
- 眼睛保护神器- [f.lux](https://justgetflux.com)
- 多功能分享神器-[ShareX](http://www.appinn.com/sharex/)
- 快速启动神器— [Launchy](http://launchy.net)

**重要申明：软件仅仅只是工具，切勿本末倒置**
