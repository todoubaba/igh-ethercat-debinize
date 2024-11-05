# Debianizer for Igh EtherCAT

## 安装工具

```bash
sudo apt install build-essential quilt
```

## 下载Igh EtherCAT源代码

```bash
wget https://gitlab.com/etherlab.org/ethercat/-/archive/1.6.2/ethercat-1.6.2.tar.gz
tar -xzmf ethercat-1.6.2.tar.gz
cd ethercat-1.6.2
```

## 下载本项目

```bash
mkdir debian
cd debian
git clone https://github.com/todoubaba/igh-ethercat-debinize .
```

## 修改配置

根据需要修改`ruels`中的内容

## 打包

```bash
cd ../
debuild
```

重新打包
```bash
make clean
debuild
```
