debian7是 ubuntu12同期的版本，可以算是比较老了，升级可以参看这个
[https://wiki.debian.org/LTS/Using](https://wiki.debian.org/LTS/Using)
```
1.修改/etc/apt/source.list

deb http://deb.debian.org/debian/ jessie main contrib non-free
deb-src http://deb.debian.org/debian/ jessie main contrib non-free

deb http://security.debian.org/ jessie/updates main contrib non-free
deb-src http://security.debian.org/ jessie/updates main contrib non-free

2.apt-get update && apt-get -V upgrade

3.apt-get dist-upgrade

4.reboot

5.apt-get autoremove
```
debian8 升级 debian9 参见
[https://www.linuxidc.com/Linux/2017-12/149050.htm](https://www.linuxidc.com/Linux/2017-12/149050.htm)
