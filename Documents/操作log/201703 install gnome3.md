http://blog.csdn.net/czwin32768/article/details/51703043



安装GNOME3

其实有一个更简单粗暴的办法是直接装 UBUNTU GNOME发行版，但是当我安装完UBUNTU16的时候，我真的不想重新装一遍系统。

所以就在原有基础上安装gnome3，很多人觉得用不习惯，其实桌面环境这个还是挺方便的。

sudo apt-get install gnome-shell
sudo apt-get install ubuntu-gnome-desktop


值得注意的是，记得要在安装gnome-shell的时候选择那个gdm，不然开机默认还是unity

sudo apt-get install unity-tweak-tool
sudo apt-get install gnome-tweak-tool

注意：安装后好丑！！！


20170320

在安装了 ubuntu 后，可以添加多个桌面环境，例如：

sudo apt-get install ubuntu-desktop ubuntu-netbook kubuntu-desktop kubuntu-netbook

在登录界面输入用户名和密码那个位置，可以选择进入系统后的不同桌面环境，

同时还可以在命令行中切换下次登录时使用的登录窗口模式：

sudo dpkg-reconfigure gdm  （把 gdm 换成 kdm 也可以） lightdm

在弹出的窗口中选择使用 gdm（gnome方式）或者 kdm（kde方式）

///
卸载掉gnome-shell主程序

    $sudo apt-get remove gnome-shell

卸载掉gnome

    $sudo apt-get remove gnome

卸载不需要的依赖关系

    $sudo apt-get autoremove

彻底卸载删除gnome的相关配置文件

    $sudo apt-get purge gnome

清理安装gnome时候留下的缓存程序软件包

    $sudo apt-get autoclean

    $sudo apt-get clean

