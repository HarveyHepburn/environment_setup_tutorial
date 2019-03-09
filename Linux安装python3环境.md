
# 简单安装

apt-get update && apt-get upgrade

apt-get install python3

apt-get install python3-pip

apt-get install python3-setuptools

# 编译安装

## 安装c语言环境,保证编译成功

```
apt-get install build-essential  
  
apt-get install make zlib*

```

## 上官网下载原包

[官网](https://www.python.org/downloads/)  

使用wget命令

## 安装编译

```
tar -xzvf Python-3.6.1.tgz -C /usr/local/src/    #src一般用来存放源码目录  
  
cd /usr/local/src/  #目录下的python-3.6.1就是解压后的源码包目录  
  
cd /usr/local/src/Python-3.6.1  

./configure --with-ssl --prefix=/usr/local/python3   #这里我选择将python安装到/usr/local/python3中  

make && make install
```

## 添加环境变量

```
export PATH=$PATH:/要添加的路径



#编辑
vim ~/.bash_profile

#bash_profile的编辑,用&&执行两条命令,或;
alias python="这里写python程序路径"
alias pip="这里写pip程序路径"

#保存修改
source ~/.bash_profile
```
