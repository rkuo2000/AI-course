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

---
### [Geforce RTX 50 series](https://www.nvidia.com/zh-tw/geforce/graphics-cards/50-series/)<br>
![](https://wp-cdn.pugetsystems.com/2025/01/Screenshot-2025-01-16-094012.png)
![](https://static.gigabyte.com/StaticFile/Image/Global/2c9319cda29065cc30ac66c4838790a6/Product/43906/png/300)

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

---
### [STMicro STM32N6 series](https://www.edomtech.com/zh-tw/product-detail/STM32N6-high-performance-microcontroller/)
#### 效能
* 1280 DMIPS / 3360 CoreMark
* Helium（M-Profile 向量延伸，MVE）：新增約 150 條指令，專為高速執行進階 DSP 與機器學習程式碼而設計
* ST Neural-ART Accelerator™：
* 針對高效能、低功耗 AI 演算法最佳化
* 運作時脈 1 GHz，提供 600 GOPS，平均能源效率達 3 TOPS/W
#### 記憶體
* 無 Flash 架構設計
* 4.2 MB 連續式內嵌 RAM
* 高速序列介面支援外部記憶體：以低腳位數、具成本效益的方式，透過 8 或 16 位元介面存取外部記憶體
* 彈性記憶體控制器（PSRAM、SDRAM、NOR、NAND）
#### 進階圖形與多媒體功能
* Chrom-ART Accelerator：2D 圖形加速
* Chrom-GRC：適用於非方形顯示器的圖形資源裁切器
* NeoChrom™ Accelerator：
* 2.5D 圖形加速，支援進階繪圖功能
* 透視校正與材質貼圖
* H.264 編碼器：720p / 1080p @ 30 fps
#### JPEG 硬體加速器：
* JPEG 壓縮與解壓縮
* 高畫質 Motion JPEG 影片播放
#### 專用影像訊號處理器（ISP）：
* 支援 500 萬畫素攝影機 @ 30 fps
* 可由同一攝影機輸入影像產生 3 種不同輸出影像
* 多種攝影機介面：MIPI CSI-2（2 lanes）、16 位元平行介面
* STM32-ISP-IQTune 工具，用於管理 ISP 調校

---
### Infineon [PSOC Edge](https://www.infineon.com/products/microcontroller/32-bit-psoc-arm-cortex/32-bit-psoc-edge-arm)
* Cortex-M55 + Helium DSP @500MHz
* Cortex-M33 @200MHz
* NNLite + Ethos™ U55-128 (4 TOPS)
* SRAM up to 5/6MB
* 2.5D GPU, MIPI-DSI/DBI
* USB, 10/100 Ethernet, CAN, SPI, UART, I2C
* Security: EPC/PSA 2 and 4

---
### Realtek [AMB82-MINI](https://www.amebaiot.com/en/amebapro2/#rtk_amb82_mini)
<p><img src="https://www.amebaiot.com/wp-content/uploads/2023/03/amb82_mini.png" width="50%" height="50%"></p><br>

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
#### Cortex-M55 + Ethos U55 @220MHz  (0.11 TOPS)
![](https://www.nuvoton.com/export/sites/nuvoton/ai/.galleries/product/NuMaker-M55M1.png)

---
### Himax [WiseEye 2 AI Processor (WE2)](https://himaxwiseeyeplus.github.io/)
![](https://hackster.imgix.net/uploads/attachments/1671436/image_8vGCB6xEjo.png?auto=compress%2Cformat&w=830&h=466.875&fit=min&dpr=1)
* Cortex-M55 + Ethos-U55 @400MHz (0.05 TOPS)
* Internal 2MB SRAMs and 512KB TCM
* External 100MHz QSPI Flash, Max 16MB(128Mb)

---
## Agent Harewares comparison
[NVIDIA® Jetson Comparison / Module Specification from Jetson Orin Series to Jetson AGX Thor Series](https://www.forecr.io/blogs/embedded-systems/nvidia-jetson-comparison)<br>

### RPi5 vs RPi4
<table>
  <tr>
    <th>項目</th>
    <th>Raspberry Pi 5</th>
    <th>Raspberry Pi 4 Model B</th>
    <th>差異重點</th>
  </tr>
  <tr>
    <td>🧠 <strong>CPU</strong></td>
    <td>四核 2.4 GHz Cortex-A76</td>
    <td>四核 1.8 GHz Cortex-A72</td>
    <td>🚀 約 2–3× 效能提升</td>
  </tr>
  <tr>
    <td>🎮 <strong>GPU</strong></td>
    <td>VideoCore VII @ 1.1 GHz</td>
    <td>VideoCore VI @ 800 MHz</td>
    <td>🎨 圖形效能更強</td>
  </tr>
  <tr>
    <td>🧮 <strong>RAM</strong></td>
    <td>4GB / 8GB LPDDR4X-4267</td>
    <td>2GB / 4GB / 8GB LPDDR4-3200</td>
    <td>⚡ 記憶體頻寬更高</td>
  </tr>
  <tr>
    <td>🖥 <strong>顯示輸出</strong></td>
    <td>雙 micro-HDMI（雙 4Kp60）</td>
    <td>雙 micro-HDMI（單 4Kp60）</td>
    <td>🖥️ 多螢幕能力提升</td>
  </tr>
  <tr>
    <td>📷 <strong>相機 / DSI</strong></td>
    <td>2 × 4-lane MIPI</td>
    <td>1 × 2-lane CSI + 1 × DSI</td>
    <td>📸 支援雙鏡頭</td>
  </tr>
  <tr>
    <td>💾 <strong>PCIe</strong></td>
    <td>1 × PCIe 2.0</td>
    <td>❌ 無</td>
    <td>🚀 可接 NVMe / SSD</td>
  </tr>
  <tr>
    <td>🔌 <strong>USB</strong></td>
    <td>2× USB3 + 2× USB2</td>
    <td>2× USB3 + 2× USB2</td>
    <td>➖ 相同</td>
  </tr>
  <tr>
    <td>🔋 <strong>電源</strong></td>
    <td>5V / 5A USB-C PD</td>
    <td>5V / 3A USB-C</td>
    <td>⚠️ Pi 5 需更高功率</td>
  </tr>
  <tr>
    <td>⭐ <strong>新功能</strong></td>
    <td>電源按鈕、RTC</td>
    <td>無</td>
    <td>👍 使用更方便</td>
  </tr>
  <tr>
    <td>🔧 <strong>I/O 架構</strong></td>
    <td>RP1 I/O 控制器</td>
    <td>SoC 內建 I/O</td>
    <td>📈 I/O 效能更佳</td>
  </tr>
</table>

---
### Mac mini-M4 OrinNano-Super vs K230
<table>
  <tr>
    <th>Feature</th>
    <th>NVIDIA Jetson Orin Nano Super</th>
    <th>Kendryte K230 (CanMV / 01Studio)</th>
  </tr>
  <tr>
    <td>🎯 <strong>Primary Focus</strong></td>
    <td>High-performance Edge AI / Generative AI</td>
    <td>Ultra-low-power Vision / Audio AI</td>
  </tr>
  <tr>
    <td>🧠 <strong>AI Performance</strong></td>
    <td>Up to <strong>67 TOPS (INT8)</strong></td>
    <td>~<strong>6 TOPS (INT8)</strong></td>
  </tr>
  <tr>
    <td>🏗 <strong>Architecture</strong></td>
    <td>ARM Cortex-A78AE + Ampere GPU</td>
    <td>Dual-core RISC-V (C908 + C908V)</td>
  </tr>
  <tr>
    <td>💻 <strong>CPU</strong></td>
    <td>1.7GHz 6-core ARM Cortex-A78AE</td>
    <td>1.6 GHz RISC-V + 800 MHz RISC-V</td>
  </tr>
  <tr>
    <td>🎮 <strong>GPU</strong></td>
    <td>1024-core NVIDIA Ampere GPU</td>
    <td>❌ None (vector processing only)</td>
  </tr>
  <tr>
    <td>🧮 <strong>RAM</strong></td>
    <td>8 GB LPDDR5</td>
    <td>512 MB – 1 GB LPDDR3/4</td>
  </tr>
  <tr>
    <td>💾 <strong>Storage</strong></td>
    <td>M.2 NVMe SSD (PCIe)</td>
    <td>microSD Card</td>
  </tr>
  <tr>
    <td>🔋 <strong>Power Budget</strong></td>
    <td>7W – 25W (configurable)</td>
    <td>Very low (battery-friendly)</td>
  </tr>
  <tr>
    <td>🧰 <strong>Software Stack</strong></td>
    <td>JetPack SDK, CUDA, TensorRT</td>
    <td>CanMV (MicroPython), RT-Smart</td>
  </tr>
  <tr>
    <td>💵 <strong>Price</strong></td>
    <td>~$249 USD (Dev Kit)</td>
    <td>~$25 – $55 USD</td>
  </tr>
</table>

---
### Mac M4 Pro vs Jetson Orin 64GB
<table>
  <tr>
    <th>Feature</th>
    <th>Apple M4 Pro (20-core GPU)</th>
    <th>Jetson AGX Orin 64GB</th>
  </tr>
  <tr>
    <td><strong>GPU Architecture</strong></td>
    <td>Custom Apple GPU architecture</td>
    <td>NVIDIA Ampere architecture</td>
  </tr>
  <tr>
    <td><strong>GPU Cores</strong></td>
    <td>20 GPU cores (~2,560 shading units est.)</td>
    <td>2,048 CUDA cores + 64 Tensor Cores</td>
  </tr>
  <tr>
    <td><strong>GPU Clock Speed</strong></td>
    <td>Up to ~1.8 GHz</td>
    <td>Up to ~1.3 GHz</td>
  </tr>
  <tr>
    <td><strong>Memory</strong></td>
    <td>Unified memory up to 64 GB, 273 GB/s bandwidth</td>
    <td>64 GB LPDDR5, 204.8 GB/s bandwidth</td>
  </tr>
  <tr>
    <td><strong>AI Performance</strong></td>
    <td>Not publicly specified (16-core Neural Engine)</td>
    <td>Up to <strong>275 TOPS (INT8)</strong></td>
  </tr>
  <tr>
    <td><strong>Ray Tracing</strong></td>
    <td>Hardware-accelerated ray tracing</td>
    <td>Hardware ray-tracing support</td>
  </tr>
  <tr>
    <td><strong>Manufacturing Process</strong></td>
    <td>3 nm</td>
    <td>8 nm</td>
  </tr>
  <tr>
    <td><strong>Power Consumption</strong></td>
    <td>~32 W (estimated)</td>
    <td>Configurable 15 W – 60 W</td>
  </tr>
</table>

---
### 🛸 NVIDIA Jetson Thor vs. 🌌 NVIDIA DGX Blackwell (GB200)

<table>
  <thead>
    <tr>
      <th style="text-align: left">Feature</th>
      <th style="text-align: left">NVIDIA Jetson Thor</th>
      <th style="text-align: left">NVIDIA DGX GB200 (Blackwell)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align: left"><strong>Primary Target</strong></td>
      <td style="text-align: left">Humanoid Robots &amp; Autonomous Machines</td>
      <td style="text-align: left">LLM Training &amp; Generative AI Inference</td>
    </tr>
    <tr>
      <td style="text-align: left"><strong>Architecture</strong></td>
      <td style="text-align: left">Blackwell GPU + Grace CPU</td>
      <td style="text-align: left">Blackwell GPU + Grace CPU</td>
    </tr>
    <tr>
      <td style="text-align: left"><strong>Form Factor</strong></td>
      <td style="text-align: left">System-on-Module (Edge)</td>
      <td style="text-align: left">Full Rack / Data Center Node</td>
    </tr>
    <tr>
      <td style="text-align: left"><strong>AI Performance</strong></td>
      <td style="text-align: left">~800 TFLOPS (FP8)</td>
      <td style="text-align: left">Up to 1.4 Exaflops (FP4 in NVL72)</td>
    </tr>
    <tr>
      <td style="text-align: left"><strong>Memory Architecture</strong></td>
      <td style="text-align: left">Unified LPDDR5X (High Bandwidth)</td>
      <td style="text-align: left">HBM3e (High Bandwidth Memory)</td>
    </tr>
    <tr>
      <td style="text-align: left"><strong>Power Consumption</strong></td>
      <td style="text-align: left">~100W - 200W (Estimated)</td>
      <td style="text-align: left">Up to 120kW per Rack</td>
    </tr>
    <tr>
      <td style="text-align: left"><strong>Cooling</strong></td>
      <td style="text-align: left">Air or Passive (Integrated)</td>
      <td style="text-align: left">Liquid Cooled</td>
    </tr>
    <tr>
      <td style="text-align: left"><strong>Key Interface</strong></td>
      <td style="text-align: left">MIPI, GMSL, Ethernet (Robotics I/O)</td>
      <td style="text-align: left">5th Gen NVLink (1.8TB/s per GPU)</td>
    </tr>
  </tbody>
</table>

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*
