---
layout: post # 指定文章佈局，通常是 post
title: PC-Softwares
date: 2025-09-02 10:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [IDE] # 文章標籤，您可以自訂
description: Colab, Notepad++, Git-for-Windows, Python3-for-Windows, LLM & ComfyUI
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## 雲端平台

### [Google Colab 新手的入門教學](https://tw.alphacamp.co/blog/google-colab)

### [Kaggle 使用教學](https://www.kaggle.com/code/qi4589746/kaggle)

---
## 程式語言

### [Python Programming](https://www.programiz.com/python-programming)

### [Python Tutorials](https://www.w3schools.com/python/python_intro.asp)

---
## 程式編輯器

### For Windows
* [Download Notepad++](https://notepad-plus-plus.org/downloads/)

### For Ubuntu / MacOS
* **nano** (for Ubuntu / MacOS)
* **vim** (for Ubuntu / MacOS)

---
## Linux作業系統模擬器

### [Git-for-Windows](https://gitforwindows.org/)

---
### [Linux Command 命令列指令與基本操作入門教學](https://blog.techbridge.cc/2017/12/23/linux-commnd-line-tutorial/)
* `ls -l` (列出目錄檔案)<br>
* `cd ~` (換目錄)<br>
* `mkdir new` (產生新檔案夾)<br>
* `rm file_name` (移除檔案)<br>
* `rm –rf directory_name` (移除檔案夾)<br>
* `df .` (顯示SSD/硬碟的用量)<br>
* `df -a` (顯示所有儲存裝置的用量)<br>
* `du –sh directory` (查看某檔案夾之儲存用量)<br>
* `free` (檢查動態記憶體用量)<br>
* `ps –a`   (列出正在執行的程序)<br>
* `kill -9 567`  (移除程序 id=567)<br>
* `cat /etc/os-release` (列出顯示檔案內容，此檔案是作業系統版本)<br>
* `vi file_name` (編輯檔案)<br>
* `nano file_name` (編輯檔案)<br>
* `clear` (清除螢幕顯示)<br>
* `history` (列出操作記錄)<br>

### [GNU / Linux 各種壓縮與解壓縮指令](https://note.drx.tw/2008/04/command.html)

---
### GPU 工具箱與函式庫
* [CUDA Toolkit](https://developer.nvidia.com/cuda-toolkit) 
  - [CUDA installation](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html)
* [CuDNN](https://developer.nvidia.com/cudnn)
  - [cuDNN installation](https://docs.nvidia.com/deeplearning/cudnn/install-guide/index.html)

---
## Python 解譯器與軟體包

### [Python3 for Windows](https://www.python.org/downloads/windows/)
* Python 3.13.7 Download Windows installer (64-bit)<br>
* Python 3.12.10 Download Windows installer (64-bit)<br>

### [Windows 如何安裝Python3.11](https://ailog.tw/lifelog/2023/01/30/win-python311/#google_vignette)

---
### Ubuntu OS
`$ python3 -V`<br>

**Ubuntu 20.04 LTS**<br>
Python 3.8.10<br>

**Ubuntu 22.04 LTS**<br>
Python 3.10.12<br>

**Ubuntu 24.04 LTS**<br>
Python 3.12.3

---
### Install Python packages 
啟動 GitBash (啟動 Linux終端機)<br>

`python3 -V`<br>
`python3 –m pip install --upgrade pip`<br>
`pip -V`<br>
`pip install jupyter`<br>
`pip install pandas`<br>
`pip install matplotlib pillow imutils`<br>
`pip install opencv-python`<br>
`pip install scikit-learn`<br>
`git clone https://github.com/rkuo2000/cv2`<br>


---
### PyTorch
#### [Get-Started](https://pytorch.org/get-started/locally/)<br>
#### [PyTorch Tutorials](https://pytorch.org/tutorials/)
`pip install torch torchvision torchaudio`<br>

---
### Tensorflow
#### [Tensorflow Turorials](https://www.tensorflow.org/tutorials)
`pip install tensorflow`<br>

---
## LLM 安裝

### [Ollama](https://ollama.com/)

* [Download](https://ollama.com/download)

* [Models](https://ollama.com/search)

* commands
  
```
ollama -h
ollama -v
ollama pull gemma3
ollama list
ollama run gemma3
```

---
### [LM Studio](https://lmstudio.ai/)
![](https://lmstudio.ai/_next/image?url=%2F_next%2Fstatic%2Fmedia%2Fhero-new.f48a84ba.webp&w=3840&q=75)

---
### [ComfyUI](https://github.com/comfyanonymous/ComfyUI)

#### [ComfyUI 安裝](https://www.comfy.org/zh-cn/download) 

#### workflow
![](https://comfyui-wiki.com/_next/static/media/ace_step_1_t2a_step_guide.a0ff569a.jpg)

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*

