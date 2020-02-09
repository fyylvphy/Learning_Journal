## 1. 在VMware上安装Ubuntu（以19.11.12安装为例）

直接搬运我在知乎上看到的[一篇文章](https://zhuanlan.zhihu.com/p/38797088)，很详细。

安装时我设置的处理器数量为2，每个处理器的核数为2. （对于20.02.09，我处理器配置了2个，每个核数为4，内存为8G,磁盘空间40G）

磁盘分区如下:

![My_partition](https://github.com/fyylvphy/Learning_Journal/raw/master/VMware/%E8%99%9A%E6%8B%9F%E6%9C%BA%E5%88%86%E5%8C%BA.JPG)

/boot为启动盘，swap area类似于Windows里的虚拟内存，/ 为根目录。


## 2. 安装VMware
见这篇[文章](https://www.cnblogs.com/DA799422035/p/9058210.html)，不要看上面的知乎。

## 3. 配置镜像源
[教程](https://blog.csdn.net/weixin_41762173/article/details/79480832)

[清华大学镜像源](https://mirrors.tuna.tsinghua.edu.cn/help/ubuntu/)

## 4. 更换shell为zsh
[教程](https://blog.csdn.net/weixin_38111667/article/details/86157841)

## 5. 安装中文输入法
```
  sudo apt-get install ibus-pinyin
```
重启后在设置里弄就行。[教程](https://www.cnblogs.com/asmer-stone/p/9069866.html)
