vBookmarks
==============

[HomePage](http://windviki.github.com/vBookmarks/)

Modified from NeatBookmarks, an excellent bookmark extension for Google Chrome. 

Clicking the Bookmark Star in Chrome is an awful way to add a bookmark, and what I need is an extension just like "AddBookmarkHere" for Firefox.
So I added some new features to "NeatBookmarks", it's easy to manage your bookmarks now.

1) Bookmark current tab before selected bookmark/folder.

2) Bookmark current tab after selected bookmark/folder.

3) Bookmark current tab to the top of selected folder.

4) Bookmark current tab to the bottom of selected folder.

5) Add a sub-folder into selected folder.

6) Update URL of selected bookmark with current URL.

7) Copy title and URL information for selected bookmarks into clipboard.

8) Add an option: only show the nodes of the Bookmark Bar.

9) Add: separators for bookmarks or folders. Cannot be synchronized.

10) Add: update checking and notification based on github. A tricky solution.

11) Fix bugs in Neat Bookmarks.

Licensed under the [MIT License](http://www.opensource.org/licenses/mit-license.php).

Read the [FAQ](https://github.com/windviki/vBookmarks/wiki/FAQ).


Attentions
-----------------

Above Chrome 20+, please drag this crx file to chrome://chrome/extensions/ to install it.

Above Chrome 22+, please add startup parameters (--enable-easy-off-store-extension-install) for Chrome.exe so that it can accept extensions which are from outside of the WebStore.

See [link](http://www.howtogeek.com/120743/how-to-install-extensions-from-outside-the-chrome-web-store/) for details.


Chinese Introduction
-----------------

增加功能：

1) 在选中的书签/文件夹之前/之后添加当前tab为新书签

2) 在选中的文件夹顶部/底部添加当前tab为新书签

3) 在选中的文件夹中添加子文件夹

4) 替换选中的书签的URL为当前tab的URL

5) 拷贝选中书签的标题和URL到剪贴板

6) 增加选项：仅在插件里显示书签工具栏中的书签

7) 增加存储于本地的书签分隔符

8) 内建的新版本提醒

9) 修正Neat Bookmarks中的已知BUG

近期版本说明：

版本1.2 在Chrome20+有双滚动条问题。

版本1.3 修正以上问题，但是Chrome20以下版本滚动条不出现。

版本1.4 彻底解决滚动条问题。

版本1.5 解决Chrome的更新引起的一些问题，推荐Chrome20以上版本使用。

版本1.6 解决CSP相关的一些问题（Omnibox搜索（地址栏里*+空格）不能使用以及弹出框大小不能记忆的问题）。

版本1.7 修正Chrome19的双滚动条问题。之前没对Chrome19进行测试，遗漏了这个版本。请Chrome19的朋友重新更新。修正根目录展开时候popup宽度重置的问题。

版本1.8 实现书签分隔符（只存在于本地，无法随书签同步）。
修正Chrome18更新以来导致的drag-drop位置不正确的问题。
更改ICON颜色。
实现一个基于Github的更新检测和提醒（没有美元信用卡开不了webstore账户的人伤不起）。
移除多国语言，仅保留en,ja,zh,zh_TW（英语，日语，简体中文，繁体中文）。

版本1.9 修正popup刚刚打开时候滚动条会被重置到顶部的bug。
更改ICON细节。
更改更新检测的细节。
修改默认分割条的样式。

版本2.0 修正版本检测。
改进分隔条的实现，现在可以和书签一起同步了（其实就是特殊标识的书签）。
增加分隔条相关的几个高级选项。


- “被用作分隔符的书签节点的标题”：默认为"|"，即通过vbookmarks菜单新建的分隔符（一个特殊书签）在Chrome自带的书签管理器或者书签栏里显示的书签标题文字。改为"------------"，可以在自带的书签菜单里起到视觉上的分割作用。


- “被用作分隔符的书签节点的URL”：默认为"http://separatethis.com/ "，即通过vbookmarks菜单新建的分隔符（一个特殊书签）在Chrome自带的书签管理器或者书签栏里显示的书签链接地址。在vbookmarks里会显示为真正的分隔条，并且不可点击。


- “如果任一书签URL含有以下字符串，将被显示为分隔符”：如果设置了该值（多个URL值用";"隔开），URL包含了该值的所有书签都会在vbookmarks里被显示为真正的分隔条。例如，设置为google.com，则所有google域名的书签都会变成分隔条。

注意：

Chrome20+ 在安装本扩展的时候，需要把crx拖动到扩展程序这个页面（chrome://chrome/extensions/）才能正常安装，否则会报错。

Chrome22+ 可能需要添加启动参数才能安装非WebStore的扩展。右击 Chrome 桌面快捷方式，选择-"属性"-"快捷方式"，然后在"目标"一栏尾部添加参数 --enable-easy-off-store-extension-install，然后再运行浏览器就可以了。

详情参见[link](http://www.guao.hk/posts/chrome-extensions-not-in-the-chrome-web-store-more-difficult-to-install.html)。

功能备注：

1.扩展支持地址栏搜索，地址栏里敲*，然后空格，就可以输入关键词进行书签内的检索。

2.（popup打开的时候）扩展支持键盘方向键（↑↓←→）进行书签/文件夹的选择，空格键或者回车键打开选中书签或者文件夹，HOME/END跳到开头或者结尾。
PAGE DOWN/UP翻页，DELETE键删除书签。

3.选中书签，文件夹的时候，F2键可编辑。

4.鼠标中键打开目录下所有书签。

5.（popup打开的时候）Ctrl+F定位到搜索栏进行书签搜索。

6.支持书签拖放进行移动。

7.选项里可选打开书签链接后popup是否关闭。是否只显示书签栏中的书签。后台打开。书签树缩放等。

8.定制分隔符颜色（高级选项）支持十六进制颜色或者RGB颜色。#00FF00和RGB(255,0,0)都是合法的。

9.请用高级选项里的定制CSS获取更丰富的外观呈现。如改变书签树的字体。* {font-family: 微软雅黑;}

10.高级选项里可定制程序图标。


Technical Details
-----------------

Neat Bookmarks was powered by [MooTools](http://mootools.net/), but is now powered by Neatools, a custom-coded smaller subset of MooTools. 
[CodeMirror](http://codemirror.net/) is used for the Custom CSS section.


Changelogs
-----------------

**ver1.0 2011/11/15**

First version.


**ver1.1 2011/11/16**

Added: option for only displaying bookmarks in Bookmark Bar.

Added: context menu for adding folder before/after bookmark/folder.

Fixed: some translations in multi-language support.


**ver1.2 2011/11/30**

Added: update selected bookmark with current URL.

Added: copy title and URL of selected bookmark to clipboard.

Fixed: after adding new bookmark or folder to a closed folder, its original children cannot be shown correctly. 

Fixed: make up some missing translations for cs(Czech).


**ver1.3 2012/05/25**

Fixed: Scrollbar glitch. https://github.com/windviki/vBookmarks/issues/1


**ver1.4 2012/06/20**

Fixed: Scrollbar problem in Chrome 18,19. https://github.com/windviki/vBookmarks/issues/2


**ver1.5 2012/06/21**

Fixed: manifest problem in Chrome 20+.

Fixed: separated script file instead of inline scripts. see Content Security Policy http://code.google.com/chrome/extensions/contentSecurityPolicy.html


**ver1.6 2012/06/24**

Fixed: Cannot search bookmarks in Omnibox (*+space). [Content Security Policy]

Fixed: Restore width of the popup window. [Content Security Policy]

Fixed: Dialogs cannot submit their forms. [Content Security Policy]


**ver1.7 2012/06/26**

Fixed: Double scrollbars in Chrome 19. Sorry for the previous untest release. I do not have many different Chromes in different versions :)

Fixed: Width resetting occured when expanding root folder. https://github.com/windviki/vBookmarks/issues/2


**ver1.8 2012/08/01**

Added: Separators for bookmarks/folders. But it is a local record and cannot be synchronized between different devices. see https://github.com/windviki/vBookmarks/issues/3

Fixed: Neatbookmarks bug: Wrong position of dragged bookmark when vertical scrollbar is scrolled down (since Chrome18).

Added: Color of icon is changed to red.

Added: Simple update checking and desktop notification.

Removed: Several languages. Only 4 locales are left: en, ja, zh, zh_TW. Cannot maintain many translations any more.


**ver1.9 2012/08/19**

Fixed: Neatbookmarks bug: Scrollbar will be reset to the top when opening and scrolling the popup down.

Updated: Color of ICON.

Updated: Style of separator.


**ver2.0 2012/11/01**

Fixed: Version checking in background.js.

Improved: Synchronizable separators.

Added: Advanced options for separator.


- "The real title of bookmark which is shown as a separator": By default it is "|". That means the separators you added in vbookmarks will be shown as a normal bookmark in Chrome bookmark manager or bookmark menu, with this title value. You can modify it to "------------" so that you can split your bookmarks horizontally even if you check your bookmarks in Chrome bookmark menu.


- "The real URL of bookmark which is shown as a separator":By default it is "http://separatethis.com/". It's a "online separator". The separators you added in vbookmarks will be shown as a normal bookmark in Chrome bookmark manager or bookmark menu, with this URL value.


- "If URL of a bookmark contains this string, it will be shown as a separator"：If you set this value (you can set several URLs joined by ";"), all bookmarks whose URL contains any of them will be shown as real separators in vbookmarks. e.g. if you set it to google.com, all google services in your bookmarks will be shown as separators.