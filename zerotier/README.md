在codespace主机上安装zerotier

准备工作（如果你会使用zerotier组网，请直接跳至实操部分）：

1. 访问 https://my.zerotier.com/ ，点击 "LOG IN / SIGN UP"，进行登录/注册

1. 点击 "Create A Network"，下方表格会多出一栏，点击一下

1. 自行修改 "Name" 和 "Description"，改 "Access Control" 为 "Private"

至此，准备工作结束

实操如下：

1. 确保你已经创建了该仓库的 **codespace**

1. 执行 "sudo su"（获取root权限）

1. 执行 "curl -s https://install.zerotier.com | sudo bash"（安装 zerotier）

1. 执行 "zerotier-one -d"（运行zerotier服务）

1. 执行 "zerotier-cli join [16位network ID]"（线上主机加入组网）

1. 个人电脑加入组网（具体操作请自行百度）

安装完成，畅快组网
