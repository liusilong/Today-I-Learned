## nodejs 安装与卸载
### 在 **ubuntu** 系统下卸载软件

今天在**ubuntu**系统中安装了 nodejs ，使用的命令是 `sudo apt-get install nodejs` 安装的版本是 `4.2.x` 但是发现版本较低，所以需要卸载系统中的 nodejs，下载命令如下：

```Linux
sudo apt-get remove --purge 软件名称
```
例如我需要卸载 nodejs 则需要执行命令

```Linux
sudo apt-get remove --purge nodejs
```
可是有的时候我们不知道要删除软件的具体名称，则可以使用命令

```Linux
dpkg --get-selections | grep ‘软件相关名称’
```
如运行 `dpkg --get-selections | grep 'node'` 就会显示系统中所有和 `node`相关的软件

### 手动下载安装 nodejs
下载地址：https://nodejs.org/dist/

这里我们以`4.7.0`版本为例

执行下载命令

```Linux
wget https://nodejs.org/dist/v4.7.0/node-v4.7.0-linux-x64.tar.gz
```

然后解压缩

```Linux
tar xvf node-v4.7.0-linux-x64.tar.gz
```

最后配置环境变量
> 编辑配置文件 vim /etc/profile

在配置文件的最后一行加入如下代码

```Linux
export PATH=/root/node-v4.7.0-linux-x64/bin:$PATH
```
> 注意路径要写对

还有一步就是刷新环境变量

```Linux
source /etc/profile
```

检测是否安装成功

```Linux
node --version

npm --version
```

