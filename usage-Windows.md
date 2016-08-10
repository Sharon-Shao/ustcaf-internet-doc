# USTCAF VPN 配置指南（Windows）

## PPTP

### Windows 10

1. 打开start（开始菜单）->Settings（设置）
2. 选择Network & Internet -> VPN
3. 点击Add a VPN connection
4. VPN Provider 选择 "Windows (built-in)"
5. Server name or address 输入所需服务器地址
6. Connection Name填写任意名称
7. VPN Type选择PPTP
8. 在下方填写用户名和密码（也可以连接时输入），点击Save
9. 保存后在Settings -> Network & Internet -> VPN 下即可点选刚添加的VPN连接。

### Windows 7

1. 右键点击右下角任务栏的网络连接图标，选择 Open Network and Sharing Center
2. 点击 Set up a new connection or network
3. 选择 Connect to a workplace
4. 选择 Use my Internet connection (VPN)
5. Internet name 输入所需服务器地址
6. Destination name 填写任意名称
7. 勾选Don't connect now; just set it up so I can connect later，点击下一步
8. 在下一步填写用户名和密码，点击Create创建连接
9. 点击Close关闭窗口，暂时不要连接
10. 在Network and Sharing Center 中点击左侧的Change Adapter Settings
11. 在Adapter页面中可以看到刚刚添加的连接，右键点击->Properties
12. 在Security选项卡下，Type of VPN 选择PPTP，Data Encryption选择Optional Encryption，点击OK完成设置
13. 右键点击连接图标可以连接和断开VPN
