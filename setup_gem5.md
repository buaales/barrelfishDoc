# 设置gem5模拟器

## 安装gem5模拟器 

### 1. install the Mercurial

```
sudo apt-get install mercurial
```

### 2. clone gem5

``` 
hg clone http://repo.gem5.org/gem5-stable
```

### 3. install Dependences

主要的依赖软件如下：

* gcc, version 4.8 or newer
* Python, version 2.6 -2.7
* SCons, version 0.98 or newer
* SWIG, version 2.0.4 or newer
* zlib, any recent version
* m4, the macro processor
* protobuf, version 2.1, optonal but highly recommended
* pydot, optional but highly recomended

重要提示(过期)：SWIG不能使用ubuntu的软件源安装（version 2.0.11）,版本过高会导致编译错误，推荐版本为2.0.7。

### 4. install gem5

```
cd gem5-stable
scons build/ARM/gem5.fast
```

添加环境变量M5_PATH:

```
export M5_PATH=/home/???/gem5
```

## 编写配置文件


下载Full System并解压到gem5文件夹中。
