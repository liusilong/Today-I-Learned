### 重命名

#### 解压文件

将 Demo 文件 压缩成 Demo.zip 文件

```Linux
zip -r Demo.zip Demo
```
将 Demo.zip 解压到 Demo2 目录

```Linux
unzip Demo.zip -d Demo2 
```
#### 重命名
linux下重命名文件或文件夹的命令mv既可以重命名，又可以移动文件或文件夹.

**将目录A重命名为B**

```Linux
mv A B
```
**将 a.txt 重命名为 b.txt**

```Linux
mv a.txt b.txt
```

**将/a目录移动到/b下，并重命名为c**

```Linux
mv /a /b/c
```

#### **安装软件**

安装 vs code

直接从vs code 官网上下载的是 `.deb` 文件，这个时候需要这样安装

```shell
sudo dpkg -i vscode.deb
```





