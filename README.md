# -vps（以下链接纯为学习，若侵权请联系！！！）
学习笔记


wget -N --no-check-certificate

chmod +x **.sh

bash ***.sh


1.启动防火墙
systemctl start firewalld 

2.禁用防火墙
systemctl stop firewalld

3.设置开机启动
systemctl enable firewalld

4.停止并禁用开机启动
sytemctl disable firewalld

5.重启防火墙
firewall-cmd --reload

6.查看状态
systemctl status firewalld或者 firewall-cmd --state

firewall-cmd --zone=public --add-port=80/tcp  --permanent
iptables -I INPUT -p tcp --dport 9000 -j ACCEPT
iptables-save > /etc/iptables.up.rules
ip route change $defrt via $(

ip route change default via $(ip route show|grep -m1 '^default'|awk '{print $3}') initcwnd 20 initrwnd 20
net.ipv4.tcp_keepalive_time = 3600
net.ipv4.tcp_keepalive_probes = 3
net.ipv4.tcp_keepalive_intvl = 30
net.ipv4.tcp_slow_start_after_idle = 0
