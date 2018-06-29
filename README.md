# python-Steganography
Python-图片隐写术

安装与运行（ubuntu16.04）
---

1、安装包

本实验用到了 pillow 这个模块，在安装它前更新源
```
$ sudo apt-get update
```

将 python3 命令使用的 python 版本切换为 3.4，然后再安装 python3-dev 和 python3-setuptools
```
$ sudo update-alternatives --install /usr/bin/python3 python3 /usr/bin/python3.4 70 --slave /usr/bin/python3m python3m /usr/bin/python3.4m
$ sudo apt-get install python3-dev python3-setuptools
```

安装 Pillow 依赖包
```
$ sudo apt-get install libtiff5-dev libjpeg8-dev zlib1g-dev \
    libfreetype6-dev liblcms2-dev libwebp-dev tcl8.6-dev tk8.6-dev python-tk
```

安装 Pillow
```
$ sudo pip3 install Pillow
```

2、运行程序

```
usage: steganography.py [-h] [-s STRING] [-m MODE] [-o OUTPUT] filename

Please choose mode(encode/decode). If you choose [encode] please enter
filename and the description of picture else please enter filename only.

positional arguments:
  filename

optional arguments:
  -h, --help            show this help message and exit
  -s STRING, --string STRING
                        Description of the picture.
  -m MODE, --mode MODE  encode or decode.
  -o OUTPUT, --output OUTPUT
                        Directory of output picture.

```
               
               

