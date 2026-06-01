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
### Nvidia

#### [NVIDIA GTC 2026 Maps Out a New Blueprint: Rubin, Feynman, and CPO Emerge as Three Key Pillars](https://eii.nat.gov.tw/ipoforum/en/news/85)
![](https://eii.nat.gov.tw/ipoforum/backend/storage/images/2734ea00-b650-4e9b-8dd0-bdfbe3d44cc3.jpg)

#### [Vera Rubin](https://www.nvidia.com/en-us/data-center/technologies/rubin/)
![](https://image.nextplatform.com/215971.webp?imageId=215971&width=960&height=492&format=jpg)
![](https://www.ithome.com.tw/sites/default/files/field/image/0106-nvidia_rubin_platform_chips-960.jpg)

#### Groq-3 LPU
![](https://developer-blogs.nvidia.com/wp-content/uploads/2026/03/Groq-3-Architecture.webp)

#### [DGX-Spark](https://www.nvidia.com/en-us/products/workstations/dgx-spark/)
Nvidia GB10 Grace Blackwell Superchip單系統晶片。GB10包含具第5代Tensor Cores及FP4精度支援的Nvidia Blackwell GPU，使DGX具備128GB記憶體，並支援最高1000 TOPS<br>
<img width="50%" height="50%" src="https://img.technews.tw/wp-content/uploads/2025/01/07130136/NVIDIA-Project-Digits-3.png">

#### [RTX Spark](https://www.pcmag.com/news/nvidia-rtx-spark-reinvent-pc-computex-2026)
![](https://i.pcmag.com/imagery/articles/011fPR30kjbZAfV4vrdQVxI-3.fit_lim.size_768x.jpg)
![](https://i.pcmag.com/imagery/articles/011fPR30kjbZAfV4vrdQVxI-10.fit_lim.size_768x.png)

---
### [Geforce RTX 50 series](https://www.nvidia.com/zh-tw/geforce/graphics-cards/50-series/)<br>
![](https://wp-cdn.pugetsystems.com/2025/01/Screenshot-2025-01-16-094012.png)
![](https://static.gigabyte.com/StaticFile/Image/Global/2c9319cda29065cc30ac66c4838790a6/Product/43906/png/300)

---
### [Google TPU v6e](https://cloud.google.com/tpu/docs/v6e?hl=zh-tw)
![](https://cloud.google.com/static/tpu/docs/images/v6e-tpu-host.png?hl=zh-tw)

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
## Edge AI

### [Nvidia Jetson](https://developer.nvidia.com/embedded/jetson-modules)
![](https://developer.nvidia.com/sites/default/files/akamai/embedded/images/jetson-agx-orin-family-4c25-p@2x.jpg)

[NVIDIA® Jetson Comparison / Module Specification from Jetson Orin Series to Jetson AGX Thor Series](https://www.forecr.io/blogs/embedded-systems/nvidia-jetson-comparison)<br>

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
[RTX Spark](https://www.mediatek.com/products/personal-computing/nvidia-rtx-spark)<br>

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

| Feature |	Pi-5 |	Mini PC (N100) |	Jetson-Super-Nano |	Mac-Mini M4 |
|---------|------|-----------------|--------------------|-------------|
| Price	  | ~€95 |	~€200          |	€399              |	€650+       |
| RAM	    | 8GB  |	16GB           |  8GB               | 16-24GB (unified) |
| AI Engine | None | CPU-only      |	67 TOPS GPU       |	~38 TOPS Neural Engine |
| Power   |	5-10W | 15-35W	       | 15W	              | 10-25W |
| Noise   |	Silent | Varies (fan) |	Silent (fanless)    |	Near-silent |
| Local LLM |	❌	 | Barely	      |✅ (quantized)	      | ✅ (up to 13B) |
| Storage |SD/NVMe HAT |	NVMe | 512GB NVMe |	256GB-2TB |

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*
