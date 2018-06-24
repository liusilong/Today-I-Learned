### 在命令行中打开目录

**打开当前目录**

```shell
nautilus .
```

**打开指定目录，如打开 workspace 目录**

```shell
nautilus workspace
```

### 解压缩

### ZIP

**压缩一个目录，如将 demo 文件夹压缩成 demo.zip**

```shell
zip -r demo.zip demo
```

**解压 demo.zip**

```shell
unzip demo.zip
```

### TAR

**将 demo 打包成 demo.tar**

```shell
tar -cvf demo.tar demo
```

**解包 demo.tar**

```shell
tar -xvf demo.tar
```

**将 demo.tar 解包到指定目录，如解包到当前目录下的 001 目录中**

```shell
tar -xvf demo.tar -C ./001
```

### TAR.GZ

将 demo 打包成 demo.tar.gz

```shell
tar -zcvf demo.tar.gz demo
```

解压 demo.tar.gz

```shell
tar -zxvf demo.tar.gz
```

解压 demo.tar.gz 到指定目录

```shell
tar -zxvf demo.tar.gz -C ./001
```

