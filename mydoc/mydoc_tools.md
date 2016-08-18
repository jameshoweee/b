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

remove src/g4server.properties completely from the git repository and then ignore it completely:

	git rm --cached src/g4server.properties

and add it to .gitignore.

keep src/g4server.properties in the git repository but ignore future changes to this file

	git update-index --assume-unchanged src/g4server.properties

If you wanna start tracking changes again run the following command:

	git update-index --no-assume-unchanged src/g4server.properties
	
### git clone --depth 1 -v 
		

## sublime3

#### OSX El Capitan with Sublime Text 3

    ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl
    ➜  ~ vi ~/.bash_profile
    export PATH=$PATH:~/usr/local/bin
    ➜  ~ source ~/.bash_profile
    ➜  ~ subl

  it works fine!


## Atom

[atom-editor-cheat-sheet](http://sweetme.at/2014/03/10/atom-editor-cheat-sheet/)

[2016-4-6 short-cut](https://gist.github.com/chrissimpkins/5bf5686bae86b8129bee)

    Com + \     隐藏左侧树
    Ctrl+Com+P  项目间切换
    Com+b       打开已打开的文件

## phpstorm

    ⌥⇧⌘L

home WIFI

  asdfqwerzxcv

## cooltext

[图片生成](https://cooltext.com/)

[]()

## vps
[王掌柜](http://since1989.org/contact)

[cnvultr](http://www.cnvultr.com/)

## java多线程

[java-multi](http://www.runoob.com/java/java-multithreading.html)

	Arrays.asList();
	Collections.rotate();
	Enumeration();

## rpc zookeeper

[huanyong](http://my.oschina.net/huangyong/blog/361751)

[zookeeper](http://www.tutorialspoint.com/zookeeper/zookeeper_fundamentals.htm)

	$ bin/zkServer.sh start

	mvn exec:java -Dexec.mainClass="com.xxx.rpc.sample.server.RpcBootstrap"

### Protobuf

	pojo

### NIO

		Netty

### nexus

	To have launchd start nexus at login:
	  ln -sfv /usr/local/opt/nexus/*.plist ~/Library/LaunchAgents
	Then to load nexus now:
	  launchctl load ~/Library/LaunchAgents/homebrew.mxcl.nexus.plist
	Or, if you don't want/need launchctl, you can just run:
	  nexus start

[私服定义](http://my.oschina.net/lujianing/blog/297128)		
