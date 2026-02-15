---
layout: post # 指定文章佈局，通常是 post
title: AI Hardwares
date: 2025-09-1 09:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [basic] # 文章標籤，您可以自訂
description: AI-chips, Edge-AI MCUs
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## AI chips

### [Top10 AI Chip Makers](https://research.aimultiple.com/ai-chip-makers/)
![](https://github.com/rkuo2000/AI-course/blob/main/assets/images/Top10_AI_Chip_Makers.png?raw=true)

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
![](https://github.com/rkuo2000/AI-course/blob/main/assets/images/Tesla-FSD-HW-architecture.png?raw=true)

---
### Nvidia
![](https://miro.medium.com/v2/resize:fit:720/format:webp/0*gPajGtDQ-yPGgyFj.gif)

#### [Nvidia Draws GPU System Roadmap Out To 2028](https://www.nextplatform.com/2025/03/19/nvidia-draws-gpu-system-roadmap-out-to-2028/)
![](https://www.nextplatform.com/wp-content/uploads/2025/03/nvidia-roadmap-2025-to-2028.jpg)

#### [Analysis of NVIDIA’s Latest Hardware: B100/B200/GH200/NVL72/SuperPod](https://www.fibermall.com/blog/nvidia-b100-b200-gh200-nvl72-superpod.htm)
![](https://www.fibermall.com/blog/wp-content/uploads/2024/04/GB200-uses-the-full-B200-chip-1024x338.png)

---
#### [DGX-Spark](https://www.nvidia.com/en-us/products/workstations/dgx-spark/)
Nvidia GB10 Grace Blackwell Superchip單系統晶片。GB10包含具第5代Tensor Cores及FP4精度支援的Nvidia Blackwell GPU，使DGX具備128GB記憶體，並支援最高1000 TOPS<br>
<img width="50%" height="50%" src="https://img.technews.tw/wp-content/uploads/2025/01/07130136/NVIDIA-Project-Digits-3.png">

#### [ASUS Ascent GX10](https://www.asus.com/tw/networking-iot-servers/desktop-ai-supercomputer/ultra-small-ai-supercomputers/asus-ascent-gx10/)<br>
<p>
<img width="30%" height="30%" src="https://www.dreamcore.com.sg/wp-content/uploads/01-ASUS_Ascent_GX10.MAIN_-1440x1440.jpg">
<img src="https://i0.wp.com/linuxgizmos.com/files/ASUS-Ascent-GX10-Peripherals.jpg?resize=450%2C209&ssl=1">
</p>

#### [GIGABYTE AI TOP ATOM](https://www.gigabyte.com/tw/AI-TOP-PC/GIGABYTE-AI-TOP-ATOM)
<img width="50%" height="50%" src="https://img.unikoshardware.com/wp-content/uploads/2025/10/GIGABYTE-AI-TOP-ATOM.webp">

---
### [Geforce RTX 50 series](https://www.nvidia.com/zh-tw/geforce/graphics-cards/50-series/)<br>
![](https://wp-cdn.pugetsystems.com/2025/01/Screenshot-2025-01-16-094012.png)
![](https://static.gigabyte.com/StaticFile/Image/Global/2c9319cda29065cc30ac66c4838790a6/Product/43906/png/300)

---
### [AMD Instinct™ MI355X GPUs](https://www.amd.com/en/products/accelerators/instinct/mi350/mi355x.html)
Built on the 4th Gen AMD CDNA™ architecture, AMD Instinct™ MI355X GPUs deliver leadership AI and HPC performance enabling high density infrastructures with 288GB HBM3E memory, 8TB/s bandwidth, and expanded FP6 and FP4 datatype support.

#### [AMD 7 GHz Zen 6 Clock Speed Target “Confirmed” – Leaker Claims](https://overclock3d.net/news/cpu_mainboard/amd-7-ghz-zen-6-clock-speed-target-confirmed-leaker-claims/)

---
### Intel Gaudi 3
#### [Intel® Gaudi® 3 AI Accelerators on IBM Cloud](https://www.ibm.com/products/gpu-ai-accelerator/intel-gaudi3)

---
### [Groq LPU](https://wow.groq.com/lpu-inference-engine/)
<p><img width="80%" height="80%" src="https://imageio.forbes.com/specials-images/imageserve/6037f9e640b8dd29ddc0607d/The-Groq-node-has-four-chips-per-card--similar-to-most-AI-startups-/960x0.png"></p>

---
### [Google TPU v6e](https://cloud.google.com/tpu/docs/v6e?hl=zh-tw)
![](https://cloud.google.com/static/tpu/docs/images/v6e-tpu-host.png?hl=zh-tw)

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
### RPi 5 + Hailo-8L 
<p><img width="50%" height="50%" src="https://i.gzn.jp/img/2024/06/04/raspberry-pi-ai-kit-npu-m2/00.jpg"></p>
* Hailo-8L (13 TOPs)
* Broadcom BCM2712 2.4GHz quad-core 64-bit Arm Cortex-A76 CPU, with Cryptographic Extension, 512KB per-core L2 caches, and a 2MB shared L3 cache

---
### MediaTek
[天璣9500](https://www.mediatek.tw/products/smartphones-2/mediatek-dimensity-9500)<br>
[天璣9400+](https://www.mediatek.tw/products/smartphones-2/mediatek-dimensity-9400plus)<br>

---
### [Kinara](https://kinara.ai/)
[Ara-2](https://kinara.ai/products/kinara-ara-2/)<br>
Kinara Ara-2 AI processor (40 TOPS)<br>

---
### 耐能 Kneron [KL730 AI Soc](https://www.kneron.com/tw/page/soc/)
* Quad ARM® Cortex™ A55 CPU。
* 內建DSP，可以加速AI模型後處理，語音處理。
* Linux和RTOS、TSMC 12 納米工藝。
* 高達4K@60fps解析度，與主流感測器的無縫 RGB Bayer 接口，多達4通道影像接口。
* 高達3.6eTOPS@int8 / 7.2eTops@int4。
* 支持Cafee、Tensorflow、Tensorflowlite、Pytorch、Keras、ONNX框架。
* 并兼容CNN、Transformer、RNN Hybrid等多種AI模型， 有更高的處理效率和精度。

---
### 堪智 Kendryte 
#### K230
* CPU : 1.6GHz & 0.8GHz Dual-core 64-bit RISC-V
* VPU: H.264/H.265 encoding/decoding up to 
* Memory & Storage: 32-bit LPDDR4/DDR4/LPDDR3/DDR3, SD3.01, eMMC 5.0.
* Display Output: 1-lane MIPI DSI, max @ 60fps.
* 3D Depth Engine (DPU): Up to resolution.
* Peripherals: 2x USB 2.0 OTG, 5x UART, 5x I2C, 6x PWM, 4-ch PDM (digital mic).
  
#### K210
* CPU : 400MHz Dual-Core 64-bit RISC-V RV64IMAFDC (RV64GC) CPU
* SRAM: 8MB Total On-Chip SRAM (6MB General Purpose + 2MB AI SRAM)
* NPU : 0.6TOPS
* APU : Supports Microphone Array (up to 8 microphones)
* 
---
### STMicro STM32N6
<p><img width="50%" height="50%" src="https://blog.st.com/wp-content/uploads/ST36104_STM32N6570-DK-with-camera-perspective-with-nappeCV-1-copy.jpg"></p>
* Cortex-M55 @800MHz
* Neural-ART1 (1~5 TOPS)
* Neural-ART2 (20~40 TOPS)

---
### Infineon [PSOC Edge](https://www.infineon.com/products/microcontroller/32-bit-psoc-arm-cortex/32-bit-psoc-edge-arm)
![](https://www.mouser.tw/images/marketingid/2025/img/122911023.png)

* Cortex-M55 + Helium DSP @500MHz
* Cortex-M33 @200MHz
* NNLite + Ethos™ U55-128 (4 TOPS)
* SRAM up to 5/6MB
* 2.5D GPU, MIPI-DSI/DBI
* USB, 10/100 Ethernet, CAN, SPI, UART, I2C
* Security: EPC/PSA 2 and 4
  
![](https://www.mouser.tw/images/marketingid/2023/microsites/158771261/2025-09-11_16-34-32.png)

---
### Realtek [AMB82-MINI](https://www.amebaiot.com/en/amebapro2/#rtk_amb82_mini)
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
  - Integrated Intelligent Engine (0.4 TOPS)
  
---
### Nuvoton [M55M1](https://www.nuvoton.com/ai/product/)
* Cortex-M55 + Ethos U55 @220MHz  (0.11 TOPS)
![](https://www.nuvoton.com/export/sites/nuvoton/ai/.galleries/product/NuMaker-M55M1.png)

---
### Himax [WiseEye 2 AI Processor (WE2)](https://himaxwiseeyeplus.github.io/)
![](https://hackster.imgix.net/uploads/attachments/1671436/image_8vGCB6xEjo.png?auto=compress%2Cformat&w=830&h=466.875&fit=min&dpr=1)
* Cortex-M55 + Ethos-U55 @400MHz (0.05 TOPS)
* Internal 2MB SRAMs and 512KB TCM
* External 100MHz QSPI Flash, Max 16MB(128Mb)

---
## HW spec comparison

### RPi5 vs RPi4
| 項目              | Raspberry Pi 5          | Raspberry Pi 4 Model B      | 差異重點             |
| --------------- | ----------------------- | --------------------------- | ---------------- |
| 🧠 **CPU**      | 四核 2.4 GHz Cortex-A76   | 四核 1.8 GHz Cortex-A72       | 🚀 約 2–3× 效能提升   |
| 🎮 **GPU**      | VideoCore VII @ 1.1 GHz | VideoCore VI @ 800 MHz      | 🎨 圖形效能更強        |
| 🧮 **RAM**      | 4GB / 8GB LPDDR4X-4267  | 2GB / 4GB / 8GB LPDDR4-3200 | ⚡ 記憶體頻寬更高        |
| 🖥 **顯示輸出**     | 雙 micro-HDMI（雙 4Kp60）   | 雙 micro-HDMI（單 4Kp60）       | 🖥️ 多螢幕能力提升      |
| 📷 **相機 / DSI** | 2 × 4-lane MIPI         | 1 × 2-lane CSI + 1 × DSI    | 📸 支援雙鏡頭         |
| 💾 **PCIe**     | 1 × PCIe 2.0            | ❌ 無                         | 🚀 可接 NVMe / SSD |
| 🔌 **USB**      | 2× USB3 + 2× USB2       | 2× USB3 + 2× USB2           | ➖ 相同             |
| 🔋 **電源**       | 5V / 5A USB-C PD        | 5V / 3A USB-C               | ⚠️ Pi 5 需更高功率    |
| ⭐ **新功能**       | 電源按鈕、RTC                | 無                           | 👍 使用更方便         |
| 🔧 **I/O 架構**   | RP1 I/O 控制器             | SoC 內建 I/O                  | 📈 I/O 效能更佳      |

---
### Mac mini-M4 OrinNano-Super vs K230
| Feature               | NVIDIA Jetson Orin Nano Super            | Kendryte K230 (CanMV / 01Studio)  |
| --------------------- | ---------------------------------------- | --------------------------------- |
| 🎯 **Primary Focus**  | High-performance Edge AI / Generative AI | Ultra-low-power Vision / Audio AI |
| 🧠 **AI Performance** | Up to **67 TOPS (INT8)**                 | ~**6 TOPS (INT8)**                |
| 🏗 **Architecture**   | ARM Cortex-A78AE + Ampere GPU            | Dual-core RISC-V (C908 + C908V)   |
| 💻 **CPU**            | 1.7GHz 6-core ARM Cortex-A78AE           | 1.6 GHz RISC-V + 800 MHz RISC-V   |
| 🎮 **GPU**            | 1024-core NVIDIA Ampere GPU              | ❌ None (vector processing only)   |
| 🧮 **RAM**            | 8 GB LPDDR5                              | 512 MB – 1 GB LPDDR3/4            |
| 💾 **Storage**        | M.2 NVMe SSD (PCIe)                      | microSD Card                      |
| 🔋 **Power Budget**   | 7W – 25W (configurable)                  | Very low (battery-friendly)       |
| 🧰 **Software Stack** | JetPack SDK, CUDA, TensorRT              | CanMV (MicroPython), RT-Smart     |
| 💵 **Price**          | ~$249 USD (Dev Kit)                      | ~$25 – $55 USD                    |

---
### Mac M4 Pro vs Jetson Orin 64GB
| Feature                   | Apple M4 Pro (20-core GPU)                          | Jetson AGX Orin 64GB               |
| ------------------------- | --------------------------------------------------- | ---------------------------------- |
| **GPU Architecture**      | Custom Apple GPU architecture                       | NVIDIA Ampere architecture         |
| **GPU Cores**             | 20 GPU cores (~2,560 shading units est.)            | 2,048 CUDA cores + 64 Tensor Cores |
| **GPU Clock Speed**       | Up to ~1.8 GHz                                      | Up to ~1.3 GHz                     |
| **Memory**                | Unified memory up to 64 GB, 273 GB/s bandwidth      | 64 GB LPDDR5, 204.8 GB/s bandwidth |
| **AI Performance**        | Not publicly specified (uses 16-core Neural Engine) | Up to **275 TOPS (INT8)**          |
| **Ray Tracing**           | Hardware-accelerated ray tracing                    | Hardware ray-tracing support       |
| **Manufacturing Process** | 3 nm                                                | 8 nm                               |
| **Power Consumption**     | ~32 W (estimated)                                   | Configurable 15 W – 60 W           |
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

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*
