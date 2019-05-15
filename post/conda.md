# conda 安装软件

## 可以快速安装各种科研软件。

2018-12-13

conda install -c electrostatics pdb2pqr

conda2py  install -c ambermd ambertools

2019-1-4

conda install -c electrostatics pdb2pqr

上述命令突然不能用了，提示

PackagesNotFoundError: The following packages are not available from current channels:

  - pdb2pqr
  - apbs
  - lapack

Current channels:

  - https://conda.anaconda.org/electrostatics/linux-64
  - https://conda.anaconda.org/electrostatics/noarch
  - https://repo.anaconda.com/pkgs/main/linux-64
  - https://repo.anaconda.com/pkgs/main/noarch
  - https://repo.anaconda.com/pkgs/free/linux-64
  - https://repo.anaconda.com/pkgs/free/noarch
  - https://repo.anaconda.com/pkgs/r/linux-64
  - https://repo.anaconda.com/pkgs/r/noarch
  - https://repo.anaconda.com/pkgs/pro/linux-64
  - https://repo.anaconda.com/pkgs/pro/noarch

conda.png

到conda网站中下载对应的压缩包就可以了，

 conda install pdb2pqr-1.5-py27_0.tar.bz2
就可以完成安装

(base) [zqchen@gpu4 programs]$ pdb2pqr_cli --version
pdb2pqr_cli (Version FIXME)

安装科研软件，可以先去conda中有没有。
### 软件安装位置
python 软件命令通常安装在D:\anaconda2py2764\Scripts; 如pip,pipenv,flask,
非python软件命令通常安装在D:\anaconda2py2764\Library\bin； 如git


