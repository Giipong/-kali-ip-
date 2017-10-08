# -kali-ip-
kali eth0
kali eth0 虚拟机的kali发现突然没了ip地址，也连不上网络了，<br>
上次的解决办法是还原虚拟机网络编辑器 这次发现可以用命令直接给虚拟机分配一个ip就好了<br>
ifconfig 发现没网 <br>
设置ip地址的命令的语法格式为： ifconfig 网络接口名称 ip地址 [netmask 子网掩码] 或 ifconfig 网络接口名称 ip地址[/掩码长度]<br>
将网卡eth0的IP地址设置为192.168.3.23，子网掩码为255.255.255.0  <br>
执行命令 ifconfig eth0 192.168.3.23 netmask 255.255.255.0 或者 ifconfig eth0 192.168.3.23/24<br>
再实施ifconfig,完成，连上了
