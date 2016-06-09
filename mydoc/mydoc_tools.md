---
title: tools
keywords: documentation theme, jekyll, technical writers, help authoring tools, hat replacements
last_updated: June 5, 2016
tags: [getting_started]
summary: "Tools & git"
sidebar: mydoc_sidebar
permalink: /mydoc_tools/
---


## GIT

### create a new repository on the command line

	echo "# task51" >> README.md
	git init
	git add README.md
	git commit -m "first commit"
	git remote add origin https://github.com/jnuc093/task51.git
	git push -u origin master

### push an existing repository from the command line

	git remote add origin https://github.com/jnuc093/task51.git
	git push -u origin master

### untrack-files-in-git-repos-without-deleting-them

[untrack-files-in-git-repos-without-deleting-them](http://www.arlocarreon.com/blog/git/untrack-files-in-git-repos-without-deleting-them/)

	echo "*.config">>.gitignore;
	git rm --cached "*.config";
	git add .;
	git commit -m "Ignoring and deleting config files." ;
	git push origin;

### sublime3

#### OSX El Capitan with Sublime Text 3

    ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
    ➜  ~ vi ~/.bash_profile
    export PATH=$PATH:~/usr/local/bin
    ➜  ~ source ~/.bash_profile
    ➜  ~ subl

  it works fine!


### Atom

    Com + \     隐藏左侧树
    Ctrl+Com+P  项目间切换
    Com+b       打开文件

## phpstorm

    ⌥⇧⌘L

home WIFI

  asdfqwerzxcv
  
## cooltext

[图片生成](https://cooltext.com/)

## vps
[王掌柜](http://since1989.org/contact)

[cnvultr](http://www.cnvultr.com/)
