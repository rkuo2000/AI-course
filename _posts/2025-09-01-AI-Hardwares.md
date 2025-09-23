---
layout: post
title: AI Hardwares
author: [Richard Kuo]
category: [Lecture]
tags: [jekyll, ai]
---

AI chips, Edge-AI, Benchrmarks, Frameworks

---
## AI chips

### [Top10 AI Chip Makers](https://research.aimultiple.com/ai-chip-makers/)
![](https://github.com/rkuo2000/AI-course/blob/main/images/Top10_AI_Chip_Makers.png?raw=true)

---
### Tesla
#### AI5
![](https://img.technews.tw/wp-content/uploads/2025/05/14100607/Tesla-AI4-800x359.jpeg)
![](https://pbs.twimg.com/media/GUAB7GNbYAAx0VN?format=jpg&name=small)
特斯拉 AI5 / HW5 下代 FSD 晶片號稱運算性能達 2,000~2,500TOPS（每秒兆次操作），是現款 HW4（約 500TOPS）晶片五倍，可支援更複雜的無監督 FSD 演算法。輝達 RTX5080 和 RTX5090（分別約為 1,500 美元和 3,000 美元）運算性能為 1,800TOPS 和 3,400TOPS。

#### [Tesla Hardware 4 (AI4) – Full Details and Latest News](https://www.autopilotreview.com/tesla-hardware-4-rolling-out-to-new-vehicles/)
![](https://www.autopilotreview.com/wp-content/uploads/2023/05/tesla-hardware-4-hw4-fsd-computer-2-image-696x405.jpg)

#### Hardware 3 (AI3) – FSD Computer
![](https://www.autopilotreview.com/wp-content/uploads/2019/11/andrej-karpathy-pytorch-conference-image-7-700x349.jpg)

**[Tesla’s Hardware & E/E Architecture](https://www.vaisakhvenugopal.com/p/inside-teslas-brain-before-cybertruck)**<br>
![](https://github.com/rkuo2000/AI-course/blob/main/images/Tesla-FSD-HW-architecture.png?raw=true)

---
### Nvidia
![](https://miro.medium.com/v2/resize:fit:720/format:webp/0*gPajGtDQ-yPGgyFj.gif)

#### [Nvidia Draws GPU System Roadmap Out To 2028](https://www.nextplatform.com/2025/03/19/nvidia-draws-gpu-system-roadmap-out-to-2028/)
![](https://www.nextplatform.com/wp-content/uploads/2025/03/nvidia-roadmap-2025-to-2028.jpg)

#### [Analysis of NVIDIA’s Latest Hardware: B100/B200/GH200/NVL72/SuperPod](https://www.fibermall.com/blog/nvidia-b100-b200-gh200-nvl72-superpod.htm)
![](https://www.fibermall.com/blog/wp-content/uploads/2024/04/GB200-uses-the-full-B200-chip-1024x338.png)

---
### [DGX-Spark](https://www.nvidia.com/en-us/products/workstations/dgx-spark/)
![](https://s4.itho.me/sites/default/files/styles/picture_size_large/public/field/image/0319-nvidia_dgx_personal_ai_supercomputers-spark-9601.jpg?itok=xkbEiLyr)

Nvidia GB10 Grace Blackwell Superchip單系統晶片。GB10包含具第5代Tensor Cores及FP4精度支援的Nvidia Blackwell GPU，使DGX具備128GB記憶體，並支援最高1000 TOPS<br>
![](https://img.technews.tw/wp-content/uploads/2025/01/07130136/NVIDIA-Project-Digits-3.png)

[ASUS Ascent GX10](https://www.asus.com/tw/networking-iot-servers/desktop-ai-supercomputer/ultra-small-ai-supercomputers/asus-ascent-gx10/)
搭載 NVIDIA® GB10 Grace Blackwell 超級晶片，提供高達 1 petaFLOP 的 AI 運算效能，並配備 **128GB** 記憶體，足以支援 2000 億（200B）參數模型的微調。

---
### [Geforce RTX 50 series](https://www.nvidia.com/zh-tw/geforce/graphics-cards/50-series/)<br>
[原價屋線上估價](https://www.coolpc.com.tw/evaluate.php)<br>
* Giga 5090OC 32GB<br>
* MSI 5080OC 16GB<br>
* Giga 5070Ti 16GB<br>
* Zotac 5060Ti 16GB<br>
![](https://github.com/rkuo2000/AI-course/blob/main/images/GPU-Gigabyte-RTX5060Ti-OC-16GB.png?raw=true)

---
### [AMD Instinct™ MI355X GPUs](https://www.amd.com/en/products/accelerators/instinct/mi350/mi355x.html)
Built on the 4th Gen AMD CDNA™ architecture, AMD Instinct™ MI355X GPUs deliver leadership AI and HPC performance enabling high density infrastructures with 288GB HBM3E memory, 8TB/s bandwidth, and expanded FP6 and FP4 datatype support.

#### [AMD 7 GHz Zen 6 Clock Speed Target “Confirmed” – Leaker Claims](https://overclock3d.net/news/cpu_mainboard/amd-7-ghz-zen-6-clock-speed-target-confirmed-leaker-claims/)

---
### Intel Gaudi 3
![](https://intelcorp.scene7.com/is/image/intelcorp/designed-for-ai-graphic:1920-1080?wid=978&hei=550&fmt=webp-alpha)

#### [Intel® Gaudi® 3 AI Accelerators on IBM Cloud](https://www.ibm.com/products/gpu-ai-accelerator/intel-gaudi3)

---
### Groq LPU
#### [The Groq LPU™ Inference Engine](https://wow.groq.com/lpu-inference-engine/)
**Paper:** [A Software-defined Tensor Streaming Multiprocessor for Large-scale Machine Learning](https://dl.acm.org/doi/pdf/10.1145/3470496.3527405)
<p><img width="80%" height="80%" src="https://imageio.forbes.com/specials-images/imageserve/6037f9807842cbd489fa3801/The-Groq-processor-is-unique--acting-as-a-single-fast-core-with-on-die-memory-/960x0.png"></p>
<p><img width="80%" height="80%" src="https://imageio.forbes.com/specials-images/imageserve/6037f9e640b8dd29ddc0607d/The-Groq-node-has-four-chips-per-card--similar-to-most-AI-startups-/960x0.png"></p>

---
### [Google TPU v6e](https://cloud.google.com/tpu/docs/v6e?hl=zh-tw)

#### [Google Cloud推第6代TPU為基礎的新版Hypercomputer](https://www.ithome.com.tw/news/165785)

---
### [Taiwan AI Cloud - 台智雲](https://tws.twcc.ai/)
Taiwan AI Cloud operates based on the strength of Taiwania 2, the supercomputer, which consists of 2,016 NVIDIA Tesla V100 32GB GPUs, delivering 9 PFLOPS of superior performance. 
![](https://tws.twcc.ai/wp-content/uploads/2023/09/Taiwania2-small.png)

![](https://tws.twcc.ai/wp-content/uploads/2025/07/AFS-Model-Service-1024x342.png)

---
## Edge AI

### [Nvidia Jetson](https://developer.nvidia.com/embedded/jetson-modules)
![](https://developer.nvidia.com/sites/default/files/akamai/embedded/images/jetson-agx-orin-family-4c25-p@2x.jpg)

---
### Jetson Thor
[Introducing NVIDIA Jetson Thor, the Ultimate Platform for Physical AI](https://developer.nvidia.com/blog/introducing-nvidia-jetson-thor-the-ultimate-platform-for-physical-ai/)<br>
![](https://blogs.nvidia.com/wp-content/uploads/2025/08/Slide2-960x540.jpeg)

![](https://developer-blogs.nvidia.com/wp-content/uploads/2025/08/humanoid-robot-hardware-software-png.webp)

---
### [NVIDIA Jetson Orin Nano Developer Kit Gets a “Super” Boost](https://developer.nvidia.com/blog/nvidia-jetson-orin-nano-developer-kit-gets-a-super-boost/)
**[NVIDIA® Jetson Orin Nano™ Super 入門套件包](https://www.icshop.com.tw/products/368030200911)**<br>
![](https://shoplineimg.com/6486dbe2afaddb00694ea79f/689d830ae7138100146a8ab2/800x.webp?source_format=jpg)

---
### MediaTek
[天璣9500](https://www.mediatek.tw/products/smartphones-2/mediatek-dimensity-9500)<br>
[天璣9400+](https://www.mediatek.tw/products/smartphones-2/mediatek-dimensity-9400plus)<br>

---
### [Kinara](https://kinara.ai/)
[Ara-2](https://kinara.ai/products/kinara-ara-2/)<br>
the Kinara Ara-2 AI processor, the leader in Edge AI acceleration. This 40 TOPS powerhouse tackles the massive compute demands of Generative AI and transformer-based models with unmatched cost-effectiveness.<br>

---
### Kneron

#### KNEO300 EdgeGPT
<p><img src="https://image-cdn.learnin.tw/bnextmedia/image/album/2023-11/img-1701333658-39165.jpg" width="50%" height="50%"></p>

#### [KL730 AI Soc](https://www.kneron.com/tw/page/soc/)
* Quad ARM® Cortex™ A55 CPU。
* 內建DSP，可以加速AI模型後處理，語音處理。
* Linux和RTOS、TSMC 12 納米工藝。
* 高達4K@60fps解析度，與主流感測器的無縫 RGB Bayer 接口，多達4通道影像接口。
* 高達3.6eTOPS@int8 / 7.2eTops@int4。
* 支持Cafee、Tensorflow、Tensorflowlite、Pytorch、Keras、ONNX框架。
* 并兼容CNN、Transformer、RNN Hybrid等多種AI模型， 有更高的處理效率和精度。

---
### Realtek

#### [AMB82-MINI](https://www.amebaiot.com/en/amebapro2/#rtk_amb82_mini)
<p><img src="https://www.amebaiot.com/wp-content/uploads/2023/03/amb82_mini.png" width="50%" height="50%"></p>
* MCU
  - Part Number: RTL8735B
  - 32-bit Arm v8M, up to 500MHz
* MEMORY
  - 768KB ROM
  - 512KB RAM
  - 16MB Flash
  - Supports MCM embedded DDR2/DDR3L memory up to 128MB
* KEY FEATURES
  - Integrated 802.11 a/b/g/n Wi-Fi, 2.4GHz/5GHz
  - Bluetooth Low Energy (BLE) 5.1
  - Integrated Intelligent Engine @ 0.4 TOPS
<iframe width="580" height="327" src="https://www.youtube.com/embed/_Kzqh6JXndo" title="AIoT: AmebaPro2 vs ESP32" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### [Nuvoton M55M1](https://www.nuvoton.com/ai/product/)
![](https://www.nuvoton.com/export/sites/nuvoton/ai/.galleries/product/NuMaker-M55M1.png)

---
### RPi 5 + Hailo-8L 
![](https://i.gzn.jp/img/2024/06/04/raspberry-pi-ai-kit-npu-m2/00.jpg)
Hailo-8L = 13 TOPs<br>
Broadcom BCM2712 2.4GHz quad-core 64-bit Arm Cortex-A76 CPU, with Cryptographic Extension, 512KB per-core L2 caches, and a 2MB shared L3 cache<br>

---
## Benchmarks

### [MLPerf](https://mlcommons.org/)
**MLPerf Inference v5.0** measures inference performance on 11 different benchmarks, including several large language models (LLMs), text-to-image generative AI, recommendation, computer vision, biomedical image segmentation, and graph neural network (GNN).

**MLPerf Training v5.0** measures the time to train on seven different benchmarks: LLM pretraining, LLM fine-tuning, text-to-image, GNN, object detection, recommendation, and natural language processing.

---
### NVIDIA Blackwell Supercharges AI Training
![](https://www.nvidia.com/content/nvidiaGDC/us/en_US/data-center/resources/mlperf-benchmarks/_jcr_content/root/responsivegrid/nv_container_copy/nv_tabs/item_1/nv_container/nv_image.coreimg.svg/1749018334254/black-llm-training-performance-chart.svg)

### [NVIDIA Blackwell Delivers up to 2.6x Higher Performance in MLPerf Training v5.0](https://developer.nvidia.com/blog/nvidia-blackwell-delivers-up-to-2-6x-higher-performance-in-mlperf-training-v5-0/)

---
### [NVIDIA’s MLPerf Benchmark Results](https://www.nvidia.com/en-us/data-center/resources/mlperf-benchmarks/)
![](https://www.nvidia.com/content/dam/en-zz/Solutions/Data-Center/resources/mlperf/hpc-charts-mlperf-training-sdchart-june.svg)

---
## Frameworks

### [PyTorch](https://pytorch.org)

### [Tensorflow](https://www.tensorflow.org)

### [Keras 3.0](https://keras.io/keras_3/)
![](https://s3.amazonaws.com/keras.io/img/keras_3/cross_framework_keras_3.jpg)

---
### [MLX](https://github.com/ml-explore/mlx)
MLX is an array framework for machine learning on Apple silicon, brought to you by Apple machine learning research.<br>
[MLX documentation](https://ml-explore.github.io/mlx/build/html/index.html)<br>

---
### TinyML
[EloquentTinyML](https://github.com/eloquentarduino/EloquentTinyML)

### [Tensorflow.js](https://www.tensorflow.org/js/demos)

### [MediaPipe](https://google.github.io/mediapipe/)

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*



