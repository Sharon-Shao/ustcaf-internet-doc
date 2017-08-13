# USTCAF VPN配置指南（Android）

## AnyConnect

1. 从[Google Play](https://play.google.com/store/apps/details?id=com.cisco.anyconnect.vpn.android.avf)安装"AnyConnect"，
或使用USTCLUG提供的[镜像apk](https://ftp.ustclug.org/software/anyconnect/com.cisco.anyconnect.vpn.android.avf-4.0.05062.apk)
2. 打开"AnyConnect"
3. 选择Connection -> Add VPN Connection...
4. Decription输入自定义名称
5. Server Address 填写 vpn.zlix.tech
6. Advanced -> Certificate 选择 Disable
7. 保存VPN配置并返回首页
8. 点击右上角，选择Settings
9. 去掉Block Untrusted Servers的勾并返回
10. 连接VPN，会有安全提示，确认证书的Serial (hex) 为 3B:8B:F3:4A:1C:3E:0F:1D:21:FB:69:78 ，点击Continue
11. 根据提示输入用户名密码
12. enjoy

## PPTP （适用Android 4.0 及以上）

1. 打开Settings->[Wireless & networks] More->VPN
2. 点击+号添加VPN profile
3. Type选择PPTP
4. Name输入自定义名称
5. Server address输入所需服务器地址
6. 点击Save保存配置
7. 点击已保存的配置，输入用户名密码，连接VPN

## OpenVPN

请先在网站上下载 OpenVPN 配置文件，文件名为 `hz.ustcaf.ovpn`。

Android 上需要安装 OpenVPN 的客户端，这里我们推荐使用开源的 OpenVPN for Android。

下载途径：

* 作者提供的[链接](http://plaisthos.de/android/ics-openvpn-latest-stable.apk)
* [Google Play](https://play.google.com/store/apps/details?id=de.blinkt.openvpn)
* [F-Droid](https://f-droid.org/repository/browse/?fdid=de.blinkt.openvpn)

在 OpenVPN for Android 右上角三个按钮中最右边一个，即是导入配置文件的按钮，点击并
导入配置文件。

