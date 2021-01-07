docker容器无法访问外网怎么办：

1、iptables -t nat -I POSTROUTING -j MASQUERADE 
2、luc--》网络--》防火墙--》转发 “接受” 
3、/etc/sysctl.conf 添加 net.ipv4.ip_forward=1 搞定收工
