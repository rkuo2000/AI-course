---
layout: post # 指定文章佈局，通常是 post
title: AI Hardwares
date: 2026-06-01 09:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [basic] # 文章標籤，您可以自訂
description: AI-chips, Edge-MCUs
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## AI chips

### Nvidia

#### [NVIDIA GTC 2026 Maps Out a New Blueprint: Rubin, Feynman, and CPO Emerge as Three Key Pillars](https://eii.nat.gov.tw/ipoforum/en/news/85)
![](https://eii.nat.gov.tw/ipoforum/backend/storage/images/2734ea00-b650-4e9b-8dd0-bdfbe3d44cc3.jpg)

#### [Vera Rubin](https://www.nvidia.com/en-us/data-center/technologies/rubin/)
![](https://image.nextplatform.com/215971.webp?imageId=215971&width=960&height=492&format=jpg)
![](https://www.ithome.com.tw/sites/default/files/field/image/0106-nvidia_rubin_platform_chips-960.jpg)

---
#### Groq-3 LPU
![](https://developer-blogs.nvidia.com/wp-content/uploads/2026/03/Groq-3-Architecture.webp)

---
#### [DGX-Spark](https://www.nvidia.com/en-us/products/workstations/dgx-spark/)
![](https://miro.medium.com/v2/resize:fit:4800/format:webp/1*nJjOfRdEly3K3v4JWbzpXg.png)

#### [RTX Spark](https://www.pcmag.com/news/nvidia-rtx-spark-reinvent-pc-computex-2026)
![](https://www.techpowerup.com/img/PxtC5I3GZohQcDkn.jpg)

---
### [Geforce RTX 50 series](https://www.nvidia.com/zh-tw/geforce/graphics-cards/50-series/)<br>
![](https://wp-cdn.pugetsystems.com/2025/01/Screenshot-2025-01-16-094012.png)
![](https://static.gigabyte.com/StaticFile/Image/Global/2c9319cda29065cc30ac66c4838790a6/Product/43906/png/300)

---
### AMD Ryzen
![](https://benchlife.info/wp-content/uploads/2026/05/ryzen-ai-max-400-series_3-799x450.jpg)

---
### [Google TPU-8](https://cloud.google.com/blog/products/compute/tpu-8t-and-tpu-8i-technical-deep-dive)
#### TPU 8t ASIC block diagram
![](https://storage.googleapis.com/gweb-cloudblog-publish/images/1_v4.max-1600x1600.png)

#### TPU 8i ASIC block diagram
![](https://storage.googleapis.com/gweb-cloudblog-publish/images/4_v1_nUZDsJM.max-1800x1800.png)

### [AWS Neuron](https://awsdocs-neuron.readthedocs-hosted.com/en/latest/about-neuron/index.html)

#### [Inferential2](https://awsdocs-neuron.readthedocs-hosted.com/en/latest/about-neuron/arch/neuron-hardware/inferentia2.html)
![](https://awsdocs-neuron.readthedocs-hosted.com/en/latest/_images/inferentia2.png)

#### [Trainium3](https://awsdocs-neuron.readthedocs-hosted.com/en/latest/about-neuron/arch/neuron-hardware/trainium3.html)
![](https://awsdocs-neuron.readthedocs-hosted.com/en/latest/_images/neuroncore-v4-overview.png)

---
### Tesla

#### AI-6

#### AI-5
![](https://img.technews.tw/wp-content/uploads/2025/05/14100607/Tesla-AI4-800x359.jpeg)
![](https://pbs.twimg.com/media/GUAB7GNbYAAx0VN?format=jpg&name=small)
特斯拉 AI5 / HW5 下代 FSD 晶片號稱運算性能達 2,000~2,500TOPS（每秒兆次操作），是現款 HW4（約 500TOPS）晶片五倍，可支援更複雜的無監督 FSD 演算法。輝達 RTX5080 和 RTX5090（分別約為 1,500 美元和 3,000 美元）運算性能為 1,800TOPS 和 3,400TOPS。

#### [Tesla’s Hardware & E/E Architecture](https://www.vaisakhvenugopal.com/p/inside-teslas-brain-before-cybertruck)
![](https://github.com/rkuo2000/AI-course/blob/main/assets/images/Tesla-FSD-HW-architecture.png?raw=true)

#### Tesla’s lane prediction model architecture
![](https://kevinchen.co/assets/blog/tesla-ai-day-2022/tesla-ai-day-fsd-lane-model-architecture.jpg)
![](https://kevinchen.co/assets/blog/tesla-ai-day-2022/tesla-ai-day-fsd-lane-model-lookup-table.jpg)

---
## Edge AI

### [Nvidia Jetson](https://developer.nvidia.com/embedded/jetson-modules)
![](https://developer.nvidia.com/sites/default/files/akamai/embedded/images/jetson-agx-orin-family-4c25-p@2x.jpg)


|                   | Jetson AGX Thor(T5000)                                           | Jetson AGX Orin 64GB                                              | Jetson Orin NX 16GB                                              | Jetson Orin Nano Super                                        | Jetson AGX Xavier                                           | Jetson Xavier NX                                              | Jetson Nano                                   |
| ----------------- | ---------------------------------------------------------------- | ----------------------------------------------------------------- | ---------------------------------------------------------------- | ------------------------------------------------------------- | ----------------------------------------------------------- | ------------------------------------------------------------- | --------------------------------------------- |
| AI Performance    | 2070 TFLOPS                                                      | 275 TOPS                                                          | 100 TOPS                                                         | 67 TOPS                                                       | 32 TOPS                                                     | 21 TOPS                                                       | 472 GFLOPS                                    |
| GPU               | 2560-core NVIDIA Blackwell architecture GPU with 96 Tensor Cores | 2048-core NVIDIA Ampere architecture GPU with 64 Tensor Cores     | 1024-core NVIDIA Ampere architecture GPU with 32 Tensor Cores    | 1024-core NVIDIA Ampere architecture GPU with 32 Tensor Cores | 512-core NVIDIA Volta architecture GPU with 64 Tensor Cores | 384-core NVIDIA Volta™ architecture GPU with 48 Tensor Cores | 128-core NVIDIA Maxwell™ architecture GPU    |
| GPU Max Frequency | 1.57 GHz                                                         | 1.3 GHz                                                           | 918 MHz                                                          | 1020 MHz                                                      | 1377 MHz                                                    | 1100 MHz                                                      | 921MHz                                        |
| CPU               | 14-core Arm® Neoverse®-V3AE 64-bit CPU 1MB L2 + 16MB L3        | 12-core NVIDIA Arm® Cortex A78AE v8.2 64-bit CPU 3MB L2 + 6MB L3 | 8-core NVIDIA Arm® Cortex A78AE v8.2 64-bit CPU 2MB L2 + 4MB L3 | 6-core Arm® Cortex®-A78AE v8.2 64-bit CPU 1.5MB L2 + 4MB L3 | 8-core NVIDIA Carmel Arm®v8.2 64-bit CPU 8MB L2 + 4MB L3   | 6-core NVIDIA Carmel Arm®v8.2 64-bit CPU 6MB L2 + 4MB L3     | Quad-Core Arm® Cortex®-A57 MPCore processor |
| CPU Max Frequency | 2.6 GHz                                                          | 2.2 GHz                                                           | 2.0 GHz                                                          | 1.7 GHz                                                       | 2.2 GHz                                                     | 1.9 GHz                                                       | 1.43GHz                                       |
| Memory            | 128GB 256-bit LPDDR5X 273GB/s                                    | 64GB 256-bit LPDDR5 204.8GB/s                                     | 16GB 128-bit LPDDR5 102.4GB/s                                    | 8GB 128-bit LPDDR5 102 GB/s                                   | 32GB 256-bit LPDDR4x 136.5GB/s                              | 8GB 128-bit LPDDR4x 59.7GB/s                                  | 4GB 64-bit LPDDR4 25.6GB/s                    |

---
### Jetson Thor
[Introducing NVIDIA Jetson Thor, the Ultimate Platform for Physical AI](https://developer.nvidia.com/blog/introducing-nvidia-jetson-thor-the-ultimate-platform-for-physical-ai/)<br>
![](https://blogs.nvidia.com/wp-content/uploads/2025/08/Slide2-960x540.jpeg)

![](https://developer-blogs.nvidia.com/wp-content/uploads/2025/08/humanoid-robot-hardware-software-png.webp)

---
### NVIDIA® [Jetson Orin Nano™ Super 入門套件包](https://www.icshop.com.tw/products/368030200911)
![](https://shoplineimg.com/6486dbe2afaddb00694ea79f/689d830ae7138100146a8ab2/800x.webp?source_format=jpg)

---
### 樹莓派 RPi-5
<p><img width="50%" height="50%" src="https://i.gzn.jp/img/2024/06/04/raspberry-pi-ai-kit-npu-m2/00.jpg"></p><br>
* Broadcom BCM2712 2.4GHz quad-core 64-bit ARM Cortex-A76 CPU, with Cryptographic Extension, 512KB per-core L2 caches, and a 2MB shared L3 cache
* Hailo-8L HAT (13 TOPs)

---
### 瑞芯微 RK3588
* CPU 架構： 4 核 Cortex-A76 (2.4GHz) + 4 核 Cortex-A55 (1.8GHz)，兼具高效能與低功耗。
* GPU： ARM Mali-G610 MC4，支援 OpenGL ES 1.1、2.0、3.2 等。
* AI 算力： 內建 6 TOPS 的 NPU，支援多種 AI 深度學習框架。
* 多媒體： 支援 8K@60fps 影音解碼與 8K@30fps 編碼，具備強大影像處理能力（ISP）。

---
### 耐能 Kneron [KL730 AI Soc](https://www.kneron.com/tw/page/soc/)
* Quad ARM® Cortex™ A55 CPU,  高達3.6eTOPS@int8 / 7.2eTops@int4
* 內建DSP，可以加速AI模型後處理，語音處理

---
### 堪智 Kendryte [K230](https://www.kendryte.com/product/k230)
* 1.6GHz & 0.8GHz Dual-core 64-bit RISC-V (6 TOPs), VPU: H.264/H.265
* 1/2GB 32-bit LPDDR4/DDR4/LPDDR3/DDR3, SD3.01, eMMC 5.0
![](https://www.cadtc.com.tw/development-board-and-peripheral-modules/images/board460x190_k230_img02.webp)

---
### STMicro [STM32N6 series](https://www.edomtech.com/zh-tw/product-detail/STM32N6-high-performance-microcontroller/)
* Cortext-M55 800MHz, Neural-ART (0.6TOPs / 3TOPs), 4.2MB Flash, H.264, JPEG

---
### Infineon [PSOC Edge](https://www.infineon.com/products/microcontroller/32-bit-psoc-arm-cortex/32-bit-psoc-edge-arm)
* Cortex-M55 + Helium DSP @500MHz, Cortex-M33 @200MHz, NNLite + Ethos™ U55-128 (4 TOPS), SRAM up to 5/6MB

---
### Realtek [AMB82-mini](https://www.amebaiot.com/en/amebapro2/#rtk_amb82_mini)
<p><img src="https://www.amebaiot.com/wp-content/uploads/2023/03/amb82_mini.png" width="50%" height="50%"></p><br>
* RTL8735B: 32-bit ARM v8M, @500MHz, 768KB ROM, 512KB RAM, 16MB Flash, DDR2/DDR3L up to 128MB, NN Engine (0.4 TOPs)
* 802.11 a/b/g/n Wi-Fi 2.4GHz/5GHz, BLE 5.1

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

![](https://github.com/rkuo2000/AI-course/blob/main/assets/images/RPi5_vs_RPi4B_comparison.png?raw=true)

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*
