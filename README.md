# -vps（以下链接纯为学习，若侵权请联系！！！）
学习笔记


wget -N --no-check-certificate

chmod +x **.sh

bash ***.sh

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
