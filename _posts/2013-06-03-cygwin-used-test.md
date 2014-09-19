---
layout:post
title:照片
summary:照片
---
{{page.title}}
=============
##vi配置
在${HOME}/.vimrc文件中加上： # 没有.vimrc文件就新建。
{%highlight Bash shell scripts%}
set number
set hlsearch
set fileencoding=utf-8
set fileencodings=ucs-bom,utf-8,cp936,gb18030,big5,euc-jp,euc-kr,latin1
 
set nocompatible
set backspace=indent,eol,start
 
syntax enable
{%endhighlight%}

******************
说明：
*syntax enable：*打开语法高亮。cygwin的vi缺省没有打开.  
*set nocompatible和set backspace：*配置backspace键，缺省backspace不起作用。  
*set fileencoding和set fileencodings：*缺省文件编码和自动识别文件编码顺序  
*set number：*显示行号  
*set hlsearch：*搜索到内容高亮  

##显示  
打开*${HOME}/.baserc文件，把 alias ll='ls -l'*这一行放开，就可以使用ll命令了.
把*alias ls='ls -hF --color=tty'*放开，可以让ls出来的结果变的有颜色.  