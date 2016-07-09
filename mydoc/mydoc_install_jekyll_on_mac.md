---
title: Mac envirement
tags: [getting_started, troubleshooting]
keywords:
summary: " "
sidebar: mydoc_sidebar
permalink: /mydoc_install_jekyll_on_mac/
---

## envirement

    // JDK
    /Library/Java/JavaVirtualMachines
            
    // Nexus             
    nexus start    
         
    //tomcat start
    /usr/local/opt/tomcat/bin/catalina start
    /usr/local/opt/tomcat/libexec/webapps
    
## GitLab

[GitLab install on MAC](https://github.com/WebEntity/Installation-guide-for-GitLab-on-OS-X)    
    //osx 启动 ldap
    osx sudo /usr/libexec/slapd
    
    LastUserID=$(dscl . -list /Users UniqueID | awk '{print $2}' | sort -n | tail -1)
    NextUserID=$((LastUserID + 1))
    sudo dscl . create /Users/git
    sudo dscl . create /Users/git RealName "GitLab"
    sudo dscl . create /Users/git hint "Password Hint"
    sudo dscl . create /Users/git UniqueID $NextUserID
    LastGroupID=$(dscl . readall /Groups | grep PrimaryGroupID | awk '{ print $2 }' | sort -n | tail -1)
    NextGroupID=$(($LastGroupID + 1 ))
    sudo dscl . create /Groups/git
    sudo dscl . create /Groups/git RealName "GitLab"
    sudo dscl . create /Groups/git passwd "*"
    sudo dscl . create /Groups/git gid $NextGroupID
    sudo dscl . create /Users/git PrimaryGroupID $NextGroupID
    sudo dscl . create /Users/git UserShell $(which bash)
    sudo dscl . create /Users/git NFSHomeDirectory /Users/git
    sudo cp -R /System/Library/User\ Template/English.lproj /Users/git
    sudo chown -R git:git /Users/git