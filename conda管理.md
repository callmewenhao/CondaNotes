## conda 管理

查看帮助：`conda -h/--help`or`conda command --help`

```shell
# -h, --help     Show this help message and exit.
```

查看conda版本：`conda -V`or`conda --version`

```shell
(base) C:\Users\zhaowenhao>conda -V
conda 4.10.3
# -V, --version  Show the conda version number and exit.
```

设置镜像源：

```shell
#设置清华镜像
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/bioconda/
#设置搜索时显示通道地址
conda config --set show_channel_urls yes
```

查看当前源：

```shell
(base) C:\Users\zhaowenhao>conda config --show-sources
==> C:\Users\zhaowenhao\.condarc <==
channels:
  - defaults
custom_channels:
  conda-forge: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  msys2: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  bioconda: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  menpo: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
  pytorch: https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud
default_channels:
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main
  - https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/r
show_channel_urls: True
```

检查更新当前conda

```shell
# 这个没试过
(base) C:\Users\zhaowenhao>conda update conda
```

