## apt依赖问题
```Bash
sudo apt install -f
sudo rm /var/cache/apt/archives/*.deb
sudo apt upgrade
```

## 安装.deb
```Bash
dpkg -i code_1.19.3-1516876437_amd64.deb
```

## 安装pip3
```Bash
apt-get install python3-pip
```

## 设置SSH允许Root登录
```Bash
sudo apt-get install openssh-server
sudo ps -ef |grep ssh
vim  /etc/ssh/sshd_config
找到#PermitRootLogin prohibit-password改为PermitRootLogin yes
/etc/init.d/ssh restart
```

## 安装系统时root密码留空
```Bash
sudo passwd
Password：你当前的密码
Enter new UNIX password：这个是root的密码 
Retype new UNIX password：重复root的密码 
```

## group 
### 添加组
```v
groupadd  [groupname]
```
### 给组添加权限(read,write,execute)(e被占着了所以用x)
```Bash
chmod -R g+rwx ./
```
### 添加某用户到组
```Bash
usermod -G kg zhaodachuan
```
### 添加用户
```Bash
useradd [name]
```

### 添加root权限
```Bash

```


## 杀僵尸进程
```Bash
sudo kill -SIGCHLD $(ps -A -ostat,ppid | awk '/[zZ]/{print $2}')
```

## rm,cp覆盖代码文件恢复
```Bash
grep -i -a -B200 -A200 'node_name_set' /dev/vdb1 > file.txt
node_name_set改成你删除的文件里的独有的字符串。

/dev/vdb1 是你文件所在的硬盘。

-B200 -A200的意思是找到这个字符串之后上下截取200行返回
```

