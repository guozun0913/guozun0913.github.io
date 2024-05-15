## yolov5+deepsort项目调试遇到的问题及解决方法

#### 1.安装PyYAML==5.3 失败 

```
1.更新setuptools：pip install --upgrade pip setuptools    未解决
```

```
2.安装5.2 pip install PyYAML==5.2                        未解决
```

```
3.查询得知可能是由于 PyYAML 包中的一些配置与 setuptools 不兼容导致的。这个问题可能需要 PyYAML 的开发者来解决。
```

#### 2.libgthread-2.0.so.0: cannot open shared object file: No such file or directory

```
apt-get update
```

```
apt-get install libglib2.0-dev
```

#### 3.Upsample' object has no attribute 'recompute_scale_factor'

#### 4.No module named 'easydict'

```
pip instlall easy dict
```

