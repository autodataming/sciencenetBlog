### anaconda

#### 版本
不同的anaconda 版本中默认自带的python 版本不一样。
Python 3.5 (Anaconda 4.2.0) or
Python 3.6 (Anaconda 5.2.0)
历史版本的anaconda
https://repo.continuum.io/archive/
最新版本不兼容pipenv ,因此推荐使用python3.6 和python2.7版本的anaconda

#### bug
python 3.7 anaconda 2019 win64 有一个bug
pip is configured with locations that require TLS/SSL, however the ssl module in Python is not available.

解决办法：
https://slproweb.com/products/Win32OpenSSL.html
Win64OpenSSL_Light-1_1_1b.exe 下载安装就可以了。
If you are on Windows and use anaconda this worked for me:

I tried a lot of other solutions which did not work (Environment PATH Variable changes ...)

The problem can be caused by DLLs in the Windows\System32 folder (e.g. libcrypto-1_1-x64.dll or libssl-1_1-x64.dll or others) placed there by other software.

The fix was installing openSSL from https://slproweb.com/products/Win32OpenSSL.html which replaces the dlls by more recent versions.






  File "D:\miniconda3py3664\lib\site-packages\pipenv\vendor\pythonfinder\models\python.py", line 417, in from_windows_launcher
    creation_dict = cls.parse(launcher_entry.info.version)
  File "D:\miniconda3py3664\lib\site-packages\pipenv\vendor\pythonfinder\_vendor\pep514tools\_registry.py", line 75, in __getattr__
    raise AttributeError(attr)
AttributeError: version

2018 开始anacond的版本号就变成了年月版本号，而目前win上的pipenv 并不兼容年份版本号，因此不建议使用年份anacond, 推荐使用anaconda5 完美兼容pipenv.

再谈pipenv ,pipenv 会自动读取电脑里各种版本的python，因此只要存在一个年份版本的anaconda,则其他所有版本的anaconda 都不可以用。


Usage Examples:
   Create a new project using Python 3.7, specifically:
   $ pipenv --python 3.7
#### 注意事项
创建一个新的环境显式指定python版本号，否则可能会导致python 不是想要的版本，并带来其他问题。
python36ana.exe -m pipenv --python 3.6


