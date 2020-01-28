# 安装Arch
## 制作u盘
UltraISO软件上面菜单栏点击文件->**打开** :找到下载的ISO文件->**启动** ->**写入硬盘影像**：直接写入

启动电脑开机时按F12

找到启动项吧usb启动调为第一项

正常启动后可以看到几行命令行

**更改字体（可选）**

setfont /usr/shar/kbd/consolefonts/LatGRkCYR.....

ip link 查看当前互联网设备（取第二个为WiFi）

ip link set wls8 up 打开wifi

iwlist wls8 scan |grep ESSID 扫描可以接收到什么wifi
连接wifi  
wpa_passphrase yyh 2224844907 > internet.conf  
生成一个文件，是一个配置文件  
wpa_supplicant -c internet.conf -i wls8 &  
用配置文件连接wifi &用来后台运行  
dhcpcd 用老动态分配ip  
ping 以下看一看是否成功  
timedatectl set-ntp true 设置时间  
fdisk -l 查看设备 fdisk：磁盘工具  
fdisk /dev/磁盘名就可以进入  
按p看分区按g创建新的分区后只有一个分区目前不会写入（不会造成任何更改）接下来创建分区
按n创建第一个分区默认1（直接回车） 起始位置默认2048（回车）设置分区大小+512M 可能会提示你之前有这个格式要不要移除选择Y 19：18






## 安装dwm
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
杨遗憾+
