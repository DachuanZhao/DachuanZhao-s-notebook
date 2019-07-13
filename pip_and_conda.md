## conda换源
参考 https://mirrors.tuna.tsinghua.edu.cn/help/anaconda/

```

#便于复制
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/msys2/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/bioconda/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/menpo/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/

conda config --set show_channel_urls yes



conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/main/
#Conda Forge
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/

#msys2
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/msys2/

#bioconda
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/bioconda/

#menpo
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/menpo/

#pytorch
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/
# for legacy win-64
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/peterjc123/
```

## pip换源

参考 https://mirrors.tuna.tsinghua.edu.cn/help/pypi/

```
#临时使用
pip install -i https://pypi.tuna.tsinghua.edu.cn/simple some-package

设为默认
修改

~/.config/pip/pip.conf (Linux)

%APPDATA%\pip\pip.ini (Windows 10) 或 

$HOME/Library/Application Support/pip/pip.conf (macOS) (没有就创建一个)，

修改 index-url至tuna，例如
[global]
index-url = https://pypi.tuna.tsinghua.edu.cn/simple
```