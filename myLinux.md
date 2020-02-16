# 安装Arch
## 制作u盘
UltraISO软件上面菜单栏点击文件->**打开** :找到下载的ISO文件->**启动** ->**写入硬盘影像**：直接写入

启动电脑开机时按F12

找到启动项吧usb启动调为第一项

正常启动后可以看到几行命令行

## 必要软件
git wget neovim xorg xorg-server yay wpa_supplicant dhcpcd nodejs ctags pip2 pip3 make sudo 


## 安装dwm
修改*config.h* 文件中脚本文件的路径和功能按键  
dwm窗口、菜单栏无法透明


suckless
安装simple terminal

开机自启动dwm
## 安装ranger
**将ranger的配置文件复制到家目录的.config文件下** :ranger --copy-config=all

**添加环境变量** ：RANGER_LOAD_DEFAULT_RC=FALSE

**commands.py** 可以添加功能（用python）

**rc.conf** 主要配置文件可以配置按键

**rifle.conf** 配置打开文件的默认程序

**scope.sh** 配置预览文件，预览视频，图片，文档。。。。

**设置上下左右移动：** 在rc.conf文件中找到*VIM-LIKE*

## 窗口透明化
**安装picom** :sudo pacman -S picom

## 设置ssh公钥

## 安装simple terminal
