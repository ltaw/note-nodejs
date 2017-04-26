# note-nodejs
nodejs和npm升级到最新版本的方法。
<h4>1.在Ubuntu系统下：</h4>
查看当前NodeJS和npm的版本：

node -v  
npm -v  
在Linux系统下使用一个叫n的包管理器来对NodeJS进行升级。

先清除npm的cache：

sudo npm cache clean -f  
安装n模块：
 
sudo npm install -g n  
直接安装NodeJS的稳定版：

sudo n stable  
或最新版：

sudo n latest  
也可以先查看所有的NodeJS版本，再选择版本号进行安装：

sudo n ls  
sudo n 6.5.0  
npm的升级可以使用命令：

npm update npm -g  
最后使用node -v 和 npm -v 查看版本是否已经升级。
<h4>2.在Windows系统下：<h4>
查看版本的命令和Ubuntu下一样。

不同的是Windows下不能使用“n”包管理器来对NodeJS进行管理，在这里我们使用一种叫“gnvm”的工具来管理（相关链接：https://github.com/Kenshin/gnvm）

将下载好的gnvm.exe放在NodeJS的安装目录下，在cmd下输入：


gnvm version  
出现gnvm的版本号即表示gnvm可正常使用。
使用命令：

gnvm update latest  
gnvm npm latest  
