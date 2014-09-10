#Windows OpenVPN Client

--------

##requirement:

- window 7/8 64 bit

--------

##配置步骤：
1. 安装openvpn-install-2.3.2-I003-x86_64.exe（管理员身份）。
2. 拷贝config目录到openvpn的安装目录，如D:\Program Files\OpenVPN。
3. 配置windows hosts文件(C:\Windows\System32\drivers\etc\hosts)，添加项`Ipv6Addr lczhou-lab`。
4. 启动位于桌面的OpenVPN GUI（管理员身份），连接即可。
5. 禁用本地连接的Ipv4协议。
