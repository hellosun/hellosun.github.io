---
layout: post
title: OSX下蓝牙重新连接
categories: ['OSX']
---
不知道为什么，有时候自己的蓝牙鼠标在系统唤醒后总是，无法自动连接。在配置里面重新打开扫描蓝牙也无法扫描到设备。这个时候用下面的两个命令可以重新启动蓝牙。

    $ sudo kextunload -b com.apple.iokit.BroadcomBluetoothHostControllerUSBTransport
    $ sudo kextload -b com.apple.iokit.BroadcomBluetoothHostControllerUSBTransport