# USTCAF VPN配置指南（iOS）

## OpenVPN

请先在网站上下载 OpenVPN 配置文件，文件名为 `hz.ustcaf.ovpn`。

### 在桌面系统中使用

在桌面系统如 GNOME、KDE 中，一般使用 Network Manager 来管理网络，所以安装相应的 Network Manager 的 OpenVPN
插件就可以很方便地在图形界面下使用 OpenVPN 了。

常见发行版中该插件的包名：

| 发行版 | 包名    |   
| ------ | ------- |
| Debian/Ubuntu | network-manager-openvpn, GNOME 用户请使用 network-manager-openvpn-gnome |
| Arch Linux | networkmanager-openvpn |

以常见的 Ubuntu 为例，系统默认使用 Unity 桌面，则使用以下命令安装插件：

```
sudo apt-get install network-manager-openvpn-gnome
```

安装完后，在 Network Manager 管理界面，选择`添加`，然后`导入VPN`，导入下载的OVPN配置文件。

### 在命令行中使用

首先安装 OpenVPN，大部分发行版中对应的包名一般就叫 openvpn。

然后在命令行中启动：

```
sudo openvpn --config hz.ustcaf.ovpn
```
