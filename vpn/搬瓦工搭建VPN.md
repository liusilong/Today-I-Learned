## 搬瓦工搭建 VPN

1.首先需要到[搬瓦工官网](https://bwh1.net/index.php)上面去购买云主机。最低配即可。

2.打开终端，连接云主机 `ssh root@IP地址 -p 端口号`

3.使用如下命令：

```
wget --no-check-certificate -O shadowsocks.sh https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocks.sh

chmod +x shadowsocks.sh

./shadowsocks.sh 2>&1 | tee shadowsocks.log
```

4.注意：如果选择的云主机是 **ubuntu** 的话可能会报错，原因可能是没有安装 `gcc` ，安装就好了。

[参考链接](https://teddysun.com/342.html/comment-page-31)