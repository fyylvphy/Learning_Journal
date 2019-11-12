# 创建虚拟环境，并让jupyter notebook在该环境下运行
注：[zsh：command not find:conda 的详细解决办法](https://www.jianshu.com/p/13f5d20e61f8)
1. 创建虚拟环境（Ubuntu）
```zsh
  conda create -n project_name
  进入虚拟环境：
  source activate project_name
  （退出环境）
  source deactivate project_name
  如果不写project_name,则默认打开（退出）base环境
  安装支持虚拟环境的插件nb_conda:
  conda install nb_conda
  conda install -n project_name ipykernel
```
2. 让jupyter notebook在该环境下运行

原本以为，当进入虚拟环境之后，再运行jupyter notebook应该是这个环境下的jupyter，
比如我默认创建一个文件，这个文件调用的编译器应该是这个虚拟环境中的编译器，实际上并不是.
当你进入jupyter新建文件之后，你会发现，并没有存在虚拟环境的名称，
以及import sys，print(sys.path)打印出来的根本就不是虚拟环境中的路径，
所以，必须要手动在jupyter notebook中添加自己创建的虚拟环境.

```zsh
  将虚拟环境写入jupyter notebook中的环境中：
  python -m ipykernel install --user --name project_name --display-name "project_name"
  注意要打双引号
```
