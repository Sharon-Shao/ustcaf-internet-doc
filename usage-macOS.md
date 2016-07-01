# USTCAF VPN配置指南（macOS）

## OpenVPN

1. 下载并安装[TunnelBlick](https://tunnelblick.net/downloads.html)
2. 下载并打开（双击）配置文件
3. 输入管理员密码，确认导入配置文件
4. 使用TunnelBlick连接到OpenVPN服务器（需要输入登录凭证）

## IKEv2（10.8 Mountain Lion or later）（部署中）

1. 打开->System Preferences->Network
2. 点击左侧的+号，新增一个网络接口
3. Interface选择VPN；VPN Type选择IKEv2；点击Create
4. 在左侧点击刚才创建的网络接口；Server Address填写所需服务器地址；Remote ID填写所需服务器地址；Local ID为空
5. 点击Authentication Settings；在下拉框中选择Username；输入用户名（即邮箱，下同）和密码。

## L2TP （部署中）

1. 打开->System Preferences->Network
2. 点击左侧的+号，新增一个网络接口
3. Interface选择VPN；VPN Type选择L2TP over IPSec；点击Create
4. 在左侧点击刚才创建的网络接口；Server Address填写所需服务器地址；Account name填写用户名
5. 点击Authentication Settings；User Authentication单选框选择Password，并输入您的密码；Machine Authentication选择Shared Secret，值为lug；点击OK。
6. 点击Advanced；**勾选Send all traffic over VPN connection**

## PPTP

1. 打开->System Preferences->Network
2. 点击左侧的+号，新增一个网络接口
3. Interface选择VPN；VPN Type选择PPTP；点击Create
4. 在左侧点击刚才创建的网络接口；Server Address填写所需服务器地址；Account name填写用户名
5. 点击Authentication Settings；User Authentication单选框选择Password，并输入您的密码；点击OK。
6. 点击Advanced；**勾选Send all traffic over VPN connection**
