---
title: LDAP
tags: [getting_started, formatting, content_types]
keywords: pages, authoring, exclusion, frontmatter
last_updated: March 20, 2016
summary: "This theme primarily uses pages. You need to make sure your pages have the appropriate frontmatter. One frontmatter tag your users might find helpful is the summary tag. This functions similar in purpose to the shortdesc element in DITA."
sidebar: mydoc_sidebar
permalink: /mydoc_pages/
---

## json2ldap

   [Setting-up-OpenLDAP](https://github.com/IntersectAustralia/acdata/wiki/Setting-up-OpenLDAP)
   
   ➜  ~ slappasswd -h {SSHA}
   New password:
   Re-enter new password:
   {SSHA}C5huyAldP08I1j6oUv22mrCkY2P/1Jb2
   ➜  ~ ldapsearch -D 'cn=admin,dc=localhost' -W -x -b 'o=unsw,dc=localhost'
   
### quickstart

   [quickstart](http://connect2id.com/products/json2ldap/quick-start)
   
    // get connect id(CID)
    ldap.connect { "host" : "192.168.1.107", "port" : 389 }
    
    // login in 
    ldap.simpleBind { "CID" : "eUCSwFvDaKVM63wCJCEaNLG-BA2x_GHhSFdsDbcvJa8", "DN" : "cn=Manager,dc=maxcrc,dc=com", "password" : "secrect" } 
    
   
   [ldap.md](https://github.com/jnuc093/demo/blob/master/blog/ldap.md)
   


## rpc zookeeper

[huanyong](http://my.oschina.net/huangyong/blog/361751)

[zookeeper](http://www.tutorialspoint.com/zookeeper/zookeeper_fundamentals.htm)

	$ bin/zkServer.sh start

Protobuf

	pojo

NIO

		Netty

## nexus

To have launchd start nexus at login:
  ln -sfv /usr/local/opt/nexus/*.plist ~/Library/LaunchAgents
Then to load nexus now:
  launchctl load ~/Library/LaunchAgents/homebrew.mxcl.nexus.plist
Or, if you don't want/need launchctl, you can just run:
  nexus start