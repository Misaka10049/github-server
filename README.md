# bt-in-github-server

白嫖github服务器

1. 创建该仓库的codespace

1. 执行"sudo su"（获取root权限）

1. 访问官网bt.cn，执行Linux万能安装脚本（命令如下）
   > if [ -f /usr/bin/curl ];then curl -sSO https://download.bt.cn/install/install_panel.sh;else wget -O install_panel.sh https://download.bt.cn/install/install_panel.sh;fi;bash install_panel.sh ed8484bec

1. 执行"sh btvip.sh"（升级到开心版，可不运行）

1. 最后执行"rm -f /www/server/panel/data/admin_path.pl"（删除面板安全入口）

安装完成，访问宝塔面板

可以多次白嫖
