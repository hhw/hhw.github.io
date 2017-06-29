---
title: VisualBox已经实现了无缝窗口整合
id: 53
categories:
  - 柒藝
date: 2008-05-14 23:33:00
tags:
---

前一段，看到VMware的下个版本规划时，描述了无缝整合的概念，即在主操作系统桌面同时无缝地显示虚拟机操作系统桌面。当时就觉得这太棒了，心痒痒的。

前几周，家里的Ubuntu下面的VirtualBox升级到SUN收购后的第一个升级版本v1.6，当时就看到宣传页面上已经写了&ldquo;Seamless Windows...&rdquo;，也没注意，升级之后，也没发现设置或单独的菜单涉及这方面。

今天突然调出VirtualBox的帮助来看，随便查了Seamless，发现居然已经实现了！

<pre>
**4.6\. Seamless windows**

With the "seamless windows" feature of VirtualBox, you can have 
the windows that are displayed within a virtual machine appear 
side by side next to the windows of your host. This feature is 
supported for the following guest operating systems (provided 
that the Guest Additions are installed):
   - Windows guests (support added with VirtualBox 1.5);
   - Linux or Solaris/OpenSolaris guests with an X.org server
     version 1.3 or higher[8] (support added with VirtualBox 1.6).

After seamless windows are enabled (see below), VirtualBox suppresses
the display of the Desktop background of your guest, allowing you to
run the windows of your guest operating system seamlessly next to the
windows of your host: 

...

To enable seamless mode, after starting the virtual machine, press 
the Host key (normally the right control key) together with "L". 
This will enlarge the size of the VM's display to the size of your 
host screen and mask out the guest operating system's background. 
To go back to the "normal" VM display (i.e. to disable seamless 
windows), press the Host key and "L" again.
</pre>

我实验了一下，太疯狂了，哈哈！

![截屏一](http://www.mediafire.com/imgbnc.php/79908173f0f71aee6043689cb604198d6g.jpg)

虚拟机启动完毕，按快捷键HOST+L之后，你就可以在Ubuntu的Gnome桌面上使用虚拟机里的XP系统，窗口无缝地在Gnome桌面上操作。好玩的是任务栏，当你的当前程序是VirtualBox的时候，XP的任务栏遮盖了Ubuntu的Gnome任务栏，但是当你点击Gnome桌面的时候，就出现了Gnome任务栏。

虚拟机仍然按照原来的共享方式访问主机的资源&mdash;&mdash;这一点不够Seamless。

再来一张：我在Ubuntu下面跑基于.net的Live Writer，嘿嘿！
![截屏二](http://www.mediafire.com/imgbnc.php/7ba0780111639bdb876a0298fcf9b1de6g.jpg)