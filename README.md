# -vps（以下链接纯为学习，若侵权请联系！！！）
学习笔记


wget -N --no-check-certificate

chmod +x **.sh

bash ***.sh

sprov-ui

wget -N --no-check-certificate https://raw.githubusercontent.com/lybil/-vps/master/ssr.sh&&chmod +x ssr.sh&&bash ssr.sh

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

开启ssh
yum install -y openssl openssh-server

vim /etc/ssh/sshd_config

22和rootlogin

启动ssh服务
systemctl start sshd.service

重启网络
service network restart

设置开机启动ssh服务
systemctl enable sshd.service
