# USTCAF VPN配置指南（iOS）

## OpenVPN

1. OpenVPN已在中国App Store下架。请先注册一个非中国区的Apple ID（比如美国区）。
2. 使用这个账号登录App Store
3. 在App Store中搜索并下载OpenVPN
4. 打开配置文件，打开程序选择OpenVPN
5. 打开OpenVPN，点击+号，确认导入配置
6. 输入用户名密码，连接。

## IKEv2（iOS 8 or later）（部署中）

1. 打开Settings->VPN->Add VPN Configuration
2. Type选择IKEv2
3. Description输入自定义名称
4. Server输入所需服务器地址
5. Remote ID输入vpn.ustclug.org
6. User Authentication选择Username
7. Username填写用户名（即邮箱，下同）
8. 点击右上角的Done，然后连接VPN

## L2TP （部署中）

1. 打开Settings->VPN->Add VPN Configuration
2. Type选择L2TP
3. Description输入自定义名称
4. Server输入所需服务器地址
5. Account填写用户名
6. Password填写密码（如不填则会每次连接时询问）
7. Secret填入ustcaf
8. 确认勾选Send All Traffic（默认勾选）
9. 点击右上角的Done，然后连接VPN

## PPTP

1. 打开Settings->VPN->Add VPN Configuration
2. Type选择PPTP
3. Description输入自定义名称
4. Server输入所需服务器地址
5. Account填写用户名
6. Password填写密码（如不填则会每次连接时询问）
7. 确认勾选Send All Traffic（默认勾选）
8. 点击右上角的Done，然后连接VPN
