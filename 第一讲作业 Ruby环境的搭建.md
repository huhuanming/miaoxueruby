如果有问题请发送邮件至 workboring@gmail.com，
我会在第一时间为你解答。

###安装前的预备知识

ruby 安装可以直接安装，也可以依赖于 Ruby 的 版本控制工具 rvm。


###Mac 环境

1.安装 RVM

在终端输入
	
	curl -L https://get.rvm.io | bash -s stable

安装后，我们可以稍微检查下，输入

	rvm -v
	
	rvm 1.24.1 (stable) by Wayne E. Seguin <wayneeseguin@gmail.com>, Michal Papis <mpapis@gmail.com> [https://rvm.io/]

= w = 我当前装的是 1.24.1 稳定版

这里安装完成后最好把 rvm 的下载源地址修改到taobao。
因为某些原因。。rvm的下载速度很慢。

修改方式，在淘宝的 ruby 镜像站有介绍 https://ruby.taobao.org/

2.安装 ruby

本系列课程中，我们默认安装的版本是 2.1.1 版

	rvm install 2.1.1

3.设置默认的ruby 版本

	
	rvm 2.0.0 --default
	

###Windows 环境

windows 环境下以前也有 ruby 的版本管理工具，叫 pik，
但这个工具现在已经不进行维护了。

所以我们现在主要使用 ruby installer 安装

ruby installer 官方网站 http://rubyinstaller.org/

ruby installer 2.1.5 64位 版下载地址

http://dl.bintray.com/oneclick/rubyinstaller/rubyinstaller-2.1.5-x64.exe?direct

###Linux 环境

Linux 下相对就复杂了点，不同的发行版不同的仓库对 ruby 的支持都不太相同，甚至连 rvm 都不一定好使。

####Ubuntu && Deepin

如果你使用的时 Ubuntu 的系统的话，你可以在终端尝试以下命名安装

	
	sudo apt-get install python-software-properties 
	sudo apt-add-repository ppa:brightbox/ruby-ng 
	sudo apt-get update 
	sudo apt-get install ruby2.1

####CentOS

先安装一个组件包

	yum groupinstall -y development
安装 rvm

	curl -L get.rvm.io | bash -s stable
	source /etc/profile.d/rvm.sh

可以通过 rvm -v 命令查看 rvm 版本

= w = 我当前装的是 1.24.1 稳定版

这里安装完成后最好把 rvm 的下载源地址修改到taobao。
因为某些原因。。rvm的下载速度很慢。
重载 rvm 然后安装 2.1.1 版

	rvm reload
	rvm install 2.1.1 
	
设置 ruby 2.1.1 为默认版本

	rvm use 2.1.1 --default
	
####Others

如果以上方法都不奏效的话，那你可以尝试下下载 ruby 源码，编译后进行安装。





