# Miniconda安装教程  
  
## 为什么用miniconda  
- 不占空间  
- ​​简化复杂包安装
- 让你更简单的用到Python  
  
---  
---  
  
# Mac的安装方法  
## 下载步骤  
1. 找到**终端**，并点击进入  

![官网页面](assets/miniconda1.png)     
  

2. 下载安装脚本  
```  
curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh
```
![官网页面](assets/miniconda2.png)  


3. 通过bash安装
```  
# 这里默认下载位置是～,如果自己下载位置在别处切换到下载目录执行脚本
bash ~/Miniconda3-latest-MacOSX-arm64.sh
```  
### 期间按回车或者yes就可以
![官网页面](assets/miniconda3.png)  


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
## 至此，安装完成