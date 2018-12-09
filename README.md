一键脚本安装shadowsocks/shadowsocksR/V2Ray + 开启bbr
---

一键脚本搭建shadowsocks/shadowsocksR/V2Ray + 设置开启自启动 + 升级内核&开启bbr加速。

## 支持系统
CentOS 6+

Debian 7+

Ubuntu 12+

## 使用教程
下载脚本
```
yum -y install git && git clone https://github.com/klightsaber/ss-fly
```
ubuntu请使用apt-get
```
apt-get -y install git && git clone https://github.com/klightsaber/ss-fly
```
## 一键安装Shadowsocks（SS和SSR二选一）
```
ss-fly/ss-fly.sh -i password 1024
```
参数说明: password替换成自己的密码，1024为ss开放的端口号
## 一键搭建shadowsocksR（SS和SSR二选一）
```
ss-fly/ss-fly.sh -ssr
```
执行完上述的脚本代码后，会进入到输入参数的界面，包括服务器端口，密码，加密方式，协议，混淆。可以直接输入回车选择默认值，也可以输入相应的值选择对应的选项
全部选择结束后，会看到如下界面，就说明搭建ssr成功了：
```
Congratulations, ShadowsocksR server install completed!
Your Server IP        :你的服务器ip
Your Server Port      :你的端口
Your Password         :你的密码
Your Protocol         :你的协议
Your obfs             :你的混淆
Your Encryption Method:your_encryption_method
 
Welcome to visit:https://shadowsocks.be/9.html
Enjoy it!
```
## 相关操作ssr命令
```启动：/etc/init.d/shadowsocks start
停止：/etc/init.d/shadowsocks stop
重启：/etc/init.d/shadowsocks restart
状态：/etc/init.d/shadowsocks status
 
配置文件路径：/etc/shadowsocks.json
日志文件路径：/var/log/shadowsocks.log
代码安装目录：/usr/local/shadowsocks
```

## 卸载ssr服务
```
./shadowsocksR.sh uninstall
```
## 相关链接
windows SSR客户端https://github.com/shadowsocks/shadowsocks-windows/releases

