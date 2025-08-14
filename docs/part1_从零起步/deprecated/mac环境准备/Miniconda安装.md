# 前言

## 环境是什么
环境就是我们用来运行知识库应用的一切"配置"

- 打个比方, 如果我们的后端是python写的, 又考虑到python没有自带连接deepseek和处理pdf的功能, 于是我们添加了A, B两个包裹分别来连接deepseek和处理pdf

- 那么我们的环境里就一定有以下"配置": 一个python 3.10, 一个A包裹, 和一个B包裹

## 为什么用miniconda
"配置"其实可以直接被安装在Windows里, 但是这会有一个严重的问题:

- 如果一个项目需要A包裹的0.5版本, 但是另一个项目需要A包裹的1.0版本, 那每次想要运行这两个项目, 都需要检查并重新安装冲突的包裹, 这太麻烦了, 不是吗?

而Miniconda是一个环境管理器, 我们可以用Miniconda为将来每一个项目创建单独的环境, 这样包裹就不会被混淆在一起了

尽管这个项目可能是你的第一个项目, Miniconda的使用仍然十分重要, 毕竟在这个教程结束后, 你就有能力开始全新的独立项目, 不是吗?

- 不占空间
- ​​简化复杂包安装
- 让你更简单的用到Python


# Miniconda安装教程

## 下载步骤
1. 找到**终端**，并点击进入

![官网页面](https://github.com/SuperSupeng/AI-Application-Development-for-Beginners/raw/main/assets/miniconda1.jpg)


2. 下载安装脚本
```
curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh
```
![官网页面](https://github.com/SuperSupeng/AI-Application-Development-for-Beginners/raw/main/assets/miniconda2.png)


3. 通过bash安装
```
# 这里默认下载位置是～,如果自己下载位置在别处切换到下载目录执行脚本
bash ~/Miniconda3-latest-MacOSX-arm64.sh
```
### 期间按回车或者yes就可以
![官网页面](https://github.com/SuperSupeng/AI-Application-Development-for-Beginners/raw/main/assets/miniconda3.png)


4. 添加下载源
```
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/pkgs/main/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/conda-forge/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/msys2/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/bioconda/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/menpo/

conda config --set show_channel_urls yes
```
![官网页面](https://github.com/SuperSupeng/AI-Application-Development-for-Beginners/raw/main/assets/miniconda4.png)


5. 我们可以用下面的指令检验miniconda是否安装完毕，如果输出conda和版本号则为安装成功~
```
conda --version
```
![官网页面](https://github.com/SuperSupeng/AI-Application-Development-for-Beginners/raw/main/assets/miniconda6.png)

至此，安装完成