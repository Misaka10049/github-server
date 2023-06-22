在codespace主机上搭建mc服务器

步骤如下：

1. 确保你已经创建了该仓库的 **codespace**

1. 执行 "sudo su"（获取root权限）

1. 执行 "cd mc"（切换到"mc"文件夹）

1. 下载对应服务器的核心（这里以 mc 1.20，paper服务器核心为例）
   > 执行 "wget https://api.papermc.io/v2/projects/paper/versions/1.20/builds/17/downloads/paper-1.20-17.jar"
   >
   > 下载完成后，建议将 "paper-1.20-17.jar" 改名为 "paper.jar"

1. 执行 "apt install openjdk-17-jdk"（安装 jdk-17）
   > 若出现 "Do you want to continue? [Y/n]" 提示，输入 "y"，回车即可
   > 
   > 安装完成后，执行 "java --version"，检查安装是否成功

1. 执行 "java -jar paper.jar"，等待第一次运行

1. 终端报错 "Failed to load eula.txt"，自动终止运行
   > 打开文件 "eula.txt"
   > 
   > 找到 "eula=false"，改为 "eula=true"

1. 再次执行 "java -jar paper.jar"，重新启动服务器

1. 输入 "stop" 关闭服务器（其余服务器命令请自行百度）

1. 安装组网（如 zerotier）或内网穿透（如向日葵）软件，畅快联机

注：zerotier 安装教程详见 /zerotier/README.md
