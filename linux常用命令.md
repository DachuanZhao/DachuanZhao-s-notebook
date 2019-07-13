## apt依赖问题
```
sudo apt install -f
sudo rm /var/cache/apt/archives/*.deb
sudo apt upgrade
```

## 安装.deb
```
dpkg -i code_1.19.3-1516876437_amd64.deb
```

## 安装pip3
```
apt-get install python3-pip
```

## 设置SSH允许Root登录
```
sudo apt-get install openssh-server
sudo ps -ef |grep ssh
vim  /etc/ssh/sshd_config
找到#PermitRootLogin prohibit-password改为PermitRootLogin yes
/etc/init.d/ssh restart
```

## 安装系统时root密码留空
```
sudo passwd
Password：你当前的密码
Enter new UNIX password：这个是root的密码 
Retype new UNIX password：重复root的密码 
```