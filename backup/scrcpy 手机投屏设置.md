手机先有数据线连接上电脑并打开手机  开发者模式  和USB调试
1、先下载软件到电脑 
官网地址：https://blog.sanshaokeji.top/wz/78.html
Github：https://github.com/Genymobile/scrcpy
2、解压软件
3、运行   scrcpy-console.bat  程序  当提示  Press Enter to continue... 后按回车健即可
4、在运行  scrcpy.exe  查看收发可以链接手机
5、在程序文件夹地址栏输入  CMD  回车
在命令提示框内输入  scrcpy.exe -d（USB有线连接）
在打开一个 CMD 窗口输入  scrcpy --tcpip  （开启无线连接）
在打开一个 CMD 窗口输入  scrcpy.exe -e   （运行无线连接）
6、新建一个文本文档 重命名为   start  （记得把后缀名改为.bat）
          start.bat
内容填入     scrcpy --tcpip=10.10.10.8   (手机IP地址）
                  scrcpy --turn-screen-off    （关闭手机屏幕）
在创建快捷方式 改名为   投屏   
把 快捷方式  复制到开始菜单目录   
C:\ProgramData\Microsoft\Windows\Start Menu\Programs
在开始菜单找到 投屏 文件  国定到开始菜单即可