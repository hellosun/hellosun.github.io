---
layout: post
title: OSX10.11 显示隐藏文件
categories: ['OSX']
---
升级到OSX 10.11 后，原来的显示隐藏文件的命令貌似不起作用了，后来发现只要killall Finder就可以了，代码如下：

```
$ defaults write com.apple.finder AppleShowAllFiles -bool true //显示隐藏文件
$ killall Finder 
```

```
$ defaults write com.apple.finder AppleShowAllFiles -bool false //不显示隐藏文件
$ killall Finder 
```
