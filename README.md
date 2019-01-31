# git-learning
[TOC]
#### 了解Git基本概念
Git 是目前世界上使用广泛的分布式版本控制系统。[官网](https://git-scm.com)

#### 掌握Git常用的命令行操作


##### 创建本地仓库、关联远程仓库
1.在本地硬盘（这里以 G:\DevWorkSpace\Git 为例）创建一个新的仓库(repository， 可以理解成被Git管理的目录)
创建仓库
> mkdir git-learning

   进入仓库
> cd git-learning

仓库初始化
> git init

此时仓库多了 **.git** 文件夹（隐藏）

![798227800e8d5e16d43f3693089c470a.png](en-resource://database/2005:0)

![de8cf61c31b33ac87d4ccb190ca39f14.png](en-resource://database/2003:0)

**注： 请确保仓库路径不包含中文，避免莫名的bug**

2.本地仓库关联远程仓库
下面关联两个远程仓库github、gitee，默认是origin 
> git remote add github git@github.com:a-yin/git-learning.git
> git remote add gitee git@gitee.com:a-yin/git-learning.git

![69bedd48e44463f95b8578104ec46710.png](en-resource://database/2007:0)



##### 创建远程仓库、克隆本地仓库
1.在远程仓库（这里以github为例）创建一个新的仓库(repository)
![c5cb47e8745bfe83f2784f51aa309564.png](en-resource://database/1995:0)

仓库创建成功
![8ad9dedbd6d9f24567eaf8ba846636bb.png](en-resource://database/1997:0)

2.从github（远程仓库）上clone到本地仓库
> git clone git@github.com:a-yin/git-learning.git

或者

> git clone https://github.com/a-yin/git-learning.git

![1bca3e5cfff76287f0a542ae80e08bf3.png](en-resource://database/1999:0)
![ee14e8a2be1cfb19029e55a98dee9b09.png](en-resource://database/2001:0)

**注：Git支持多种协议，默认 **git:// (原生速度最快)，其它协议得看具体情况选择使用。**


##### 本地仓库pull、push远程仓库
本地 pull 远程
> git pull github master

本地 push 远程
> git add test.txt
> git push github master

![dcca1b23c53d40f152679d5e2ae11da4.png](en-resource://database/2009:0)

****



created by lingb on 2019.01.31