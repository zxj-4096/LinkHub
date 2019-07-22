列出所有已安装软件
  2 apt list --installed
  3 安装shadowsocks
  4 sudo apt-get install python-pip
  5 pip install shadowsocks
  6 加密报错使用如下命令
  7 sudo apt install libsodium-dev
  8 pip install https://github.com/shadowsocks/shadowsocks/archive/master.zip -U
  9 
 10 tcp加速
 11 cat /proc/sys/net/ipv4/tcp_fastopen
 12 读出的结果是0或1或2或3，如果没有设置，一般都是1。现在的目的是显示3.
 13 sudo vi /etc/sysctl.conf 中添加
 14 net.ipv4.tcp_fastopen=3
 15 刷新下
 16 sudo sysctl -p
 17 
 18 
# LinkHub
