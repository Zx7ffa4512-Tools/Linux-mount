mount
=====
1.挂载windows共享发方法
--------------------------------
简单:<br/>

    mount //192.168.0.100/Temp /share/100

全部:<br/>
win机d:/folder/share的共享名为 share , 有用户administrator ,密码123在linux机上,把share挂到/mnt目录:<br/>

    mount -t cifs -o username=administrator,password=123 //192.168.0.100/share /mnt
