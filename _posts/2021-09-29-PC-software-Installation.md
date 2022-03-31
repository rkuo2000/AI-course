---
layout: post
title: PC Software Installation
author: [Richard Kuo]
category: [Lecture]
tags: [jekyll, ai]
---

PC Software Installation: Editor, GitBash, Python3.9, Anaconda3, CUDA & CuDNN, Tensorflow & PyTorch installation. 

---
## PC Software Installation
1. Editor
2. OS
3. Python
4. Tensorflow/Pytorch

---
### Editor
**Notepad++** (for Windows)<br>
Download from [https://notepad-plus-plus.org/downloads/](https://notepad-plus-plus.org/downloads/)

**nano** (for Linux)<br>
**vim** (for Linux)<br>

---
### Terminal
**Git for Windows**<br>
Download from [https://gitforwindows.org/](https://gitforwindows.org/)

**Terminal for Linux**<br>

**[Linux Command 命令列指令與基本操作入門教學](https://blog.techbridge.cc/2017/12/23/linux-commnd-line-tutorial/)**<br>
`ls` (列出目錄檔案)<br>
`cd ~` (換目錄)<br>
`mkdir new` (產生新檔案夾)<br>
`rm file_name` (移除檔案)<br>
`rm –rf directory_name` (移除檔案夾)<br>
`df .` (顯示SD卡已用量)<br>
`du –sh directory` (查看某檔案夾之儲存用量)<br>
`free` (檢查動態記憶體用量)<br>
`ps –a`   (列出正在執行的程序)<br>
`kill -9 567`  (移除程序 id=567)<br>
`cat /etc/os-release` (列出顯示檔案內容，此檔案是作業系統版本)<br>
`vi file_name` (編輯檔案)<br>
`nano file_name` (編輯檔案)<br>
`clear` (清除螢幕顯示)<br>
`history` (列出操作記錄)<br>

---
### Python3.9
**Python for Windows**<br>
* Go to [https://www.python.org/downloads/windows/](https://www.python.org/downloads/windows/)
* Download [Windows embeddable package (64-bit)](https://www.python.org/ftp/python/3.9.12/python-3.9.12-embed-amd64.zip) of Python3.9.12
* [新手踏入Python第零步-安裝Python3.9](https://www.codingspace.school/blog/2021-04-07)
* **Customomize installation** to set directory to `C:\Python39`
![](https://www.codingspace.school/static/blog/img/content/2021-04-07/vzR7KLP.webp)

**Anaconda3**<br>
* Download [Anaconda3 installer for Windows](https://docs.anaconda.com/anaconda/install/hashes/win-3-64/)
* [Windows10 安裝 Anaconda 環境](https://ithelp.ithome.com.tw/articles/10229662)<br>

---
### Nvidia GPU acceleration
* CUDA 11.6 & cuDNN 8.3.3
* [CUDA installation](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html)
* [cuDNN installation](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html)

---
### PyTorch
[PyTorch get-started](https://pytorch.org/get-started/locally/)<br>
`pip3 install torch torchvision`<br>

### Tensorflow
**using Pip**<br>
`pip3 install tensorflow`<br>
or
`pip3 install tensorflow-gpu`<br>

**using Anaconda**<br>
`conda activate tensor`<br>
`conda install tensorflow`<br>


*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*
