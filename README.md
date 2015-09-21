#Sublime Text Setup

##Structure

`/user` is the `Packages/user`, contains all my sublime text user settings

##install

[ubuntu](http://askubuntu.com/questions/172698/how-do-i-install-sublime-text-2-3)

OS X command line
`ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" ~/bin/subl`

###package Control

[install package control](https://packagecontrol.io/installation#st3)

##Theme

I am using `soda-dark`

##Sublime tricks

1.布局设置
点击菜单"View -> Layout", 可以将窗口设置成1~4行，或者两列，或者四格，方便各种开发的需要。
2.快速定位
按下快捷键ctrl+p能进行快速定位，包括文件，方法，行。不同的定位标记如下
```
file  // 无标记表示查询文件
@function  // 定位方法
:lineNum  // 定位文件的某一行
file:lineNum  // 定位到file文件中的第lineNum行
```
3.多行编辑
编写代码时，有时需要进行多行同时编辑。sublime text中选中多行并按下ctrl+shift+l，就能同时编辑多行。
或者ctrl+鼠标也能选中多行进行编辑。
4.自定义皮肤
sublime text默认使用Monokai主题。并且自带了n多主题。如果不喜欢默认主题，可以到网上去搜索主题并下载。
点击Preferences -> Browse Packages打开packages目录。将下载的文件放入Color Scheme - Default中。
在菜单Preferences -> Color Scheme中选中刚添加的文件名。重启浏览器，那么文件就使用新主题进行高亮。
如果想自己设计主题，可以到 http://tmtheme-editor.herokuapp.com/ 这个网页中进行设计。我基于默认主题
修改了一个主题，主要添加了Markdown高亮的支持，并将光标所在行和选中文字的背景弄的更加突出。
可以在这里下载。
5. 项目列表
sublime text可以添加一个目录到左侧，单做一个项目来开发。可以通过Project -> Add Folders to Project 来添加。
有时候文件夹目录与系统目录会不一致，只要选中文件夹，点击菜单Project -> Refresh Folders就能更新文件夹。
6. 代码片段
sublime text可以自己添加一些常用的代码片段，方便开发时的使用。点击菜单Tools -> New Snippet，会打开一个代码片段的编辑文件。
```
<snippet>
  <content><![CDATA[
function() {

}
]]></content>
  <!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
  <!-- <tabTrigger>hello</tabTrigger> -->
  <tabTrigger>fn</tabTrigger>
  <!-- Optional: Set a scope to limit where the snippet will trigger -->
  <!-- <scope>source.python</scope> -->
</snippet>
```
snippet表示一个代码片段。其中content是片段的正文。tabTrigger是显示该片段的代码。scope是该片段作用的文件。
编写好后，比如上面的例子就是一个新建方法的片段。保存文件到Pacakage/User目录下。
在需要只用该片段的地方输入fn再按下TAB键，文档中就会输出content中的内容。

Goto
一共有四种 Goto ：
`cmd+p` `文件定位
`cmd+;`` 词语定位 #
`cmd+r` 函数定位 @
`cmd+g` 行号定位 :

##Packages

- alignment
- ConvertToUTF8
- Terminal
    + `ctrl + shift + t` open terminal
- BracketHighlighter
    + settings file is `/user/bh_core.sublime-settings`
- Markdown Extended
- Markdown Preview
    + add user keymap `{ "keys": ["alt+m"], "command": "markdown_previe
- [SublimeTmpl](https://github.com/kairyou/SublimeTmpl)
- [SublimeCodeIntel](http://sublimecodeintel.github.io/SublimeCodeIntel/)
- [docblockr](https://github.com/spadgos/sublime-jsdocs)
- [SideBarEnhancements](https://sublime.wbond.net/packages/SideBarEnhancements)
- [Anaconda](https://sublime.wbond.net/packages/Anaconda)
    + similar as sublimecodeintel
- [Djaneiro](https://sublime.wbond.net/packages/Djaneiro)
- [SublimeLinter](https://sublime.wbond.net/packages/SublimeLinter)
- [prettify](https://github.com/victorporof/Sublime-HTMLPrettify)
- [Tag](https://github.com/SublimeText/Tag)
- [autoFileName](https://github.com/BoundInCode/AutoFileName)
- [modific](https://github.com/gornostal/Modific)
- [AndyPython](https://github.com/agibsonsw/AndyPython)
- [git](https://github.com/kemayo/sublime-text-git)
- [gitgutter](https://github.com/kemayo/sublime-text-git)

##Package Usage Resources

###Emmet

[Emmet:HTML/CSS](http://www.iteye.com/news/27580)

##JsFormat

`format javascript`

##Prettify

`ctrl + shitf + p`, then `htmlprettify`

For other plugins, you can refer to their github pages

##Reference

- [sublime text - python/java/markdown](http://zhenchen.me/technology/2014/11/05/sublime-text-introduction.html)
- [mac sublime text](http://www.jianshu.com/p/25cdc7d608bb)
- [sublime text plugins](https://wido.me/sunteya/sublime-text-packages-and-settings/)
- [sublime text配置与使用](https://github.com/chenhao-ch/blog/issues/1)
- [为 Sublime Text 3 设置 Python 的全栈开发环境](http://python.jobbole.com/81312/)
    + Setup in MAC environment
- [jikeytang/sublime-text](https://github.com/jikeytang/sublime-text)
