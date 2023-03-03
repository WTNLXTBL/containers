&emsp;此脚本用于在termux中运行unshare&chroot或proot系统。     
> &emsp;chroot系统限制更少，速度更快，在unshare后有一定安全性，不过为防止误删请勿挂载/sdcard到容器，否则可能导致数据丢失。非特殊情况请勿关闭SELinux!      

### 安装教程:             
```sh
git clone https://github.com/WTNLXTBL/containers
cd containers/package
chmod -R 755 DEBIAN
chmod 777 data/data/com.termux/files/usr/bin/container
dpkg -b . ~/containers.deb
apt update
apt install ~/containers.deb
```
