---
layout: post # 指定文章佈局，通常是 post
title: Generative Video
date: 2026-06-06 09:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [AIGC] # 文章標籤，您可以自訂
description: Image-to-Video, Text-to-Video, World-Model
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## [李宏毅_生成式導論 2024](https://www.youtube.com/playlist?list=PLJV_el3uVTsPz6CTopeRp2L2t4aL_KgiI)
[李宏毅_生成式導論 2024_第17講：有關影像的生成式AI (上) — AI 如何產生圖片和影片 (Sora 背後可能用的原理)](https://hackmd.io/@shaoeChen/rJQ89maVR)<br>
<iframe width="1026" height="578" src="https://www.youtube.com/embed/5H2bVEmYDNg" title="【生成式AI導論 2024】第17講：有關影像的生成式AI (上) — AI 如何產生圖片和影片 (Sora 背後可能用的原理)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

[李宏毅_生成式導論 2024_第18講：有關影像的生成式AI (下) — 快速導讀經典影像生成方法 (VAE, Flow, Diffusion, GAN) 以及與生成的影片互動](https://hackmd.io/@shaoeChen/HJBNLFqV0)<br>
<iframe width="1026" height="578" src="https://www.youtube.com/embed/OYN_GvAqv-A" title="【生成式AI導論 2024】第18講：有關影像的生成式AI (下) — 快速導讀經典影像生成方法 (VAE, Flow, Diffusion, GAN) 以及與生成的影片互動" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### Open-VCLIP
#### Paper: [Open-VCLIP: Transforming CLIP to an Open-vocabulary Video Model via Interpolated Weight Optimization](https://arxiv.org/abs/2302.00624)
#### Paper: [Building an Open-Vocabulary Video CLIP Model with Better Architectures, Optimization and Data](https://arxiv.org/abs/2310.05010)
#### Code: [https://github.com/wengzejia1/Open-VCLIP/](https://github.com/wengzejia1/Open-VCLIP/)
![](https://github.com/wengzejia1/Open-VCLIP/blob/main/figures/firstpage.png?raw=true)

--- 
## Text-to-Video
![](https://arxiv.org/html/2402.17177v3/extracted/2402.17177v3/figures/history.png)

[Awesome Video Diffusion Models](https://github.com/ChenHsing/Awesome-Video-Diffusion-Models)<br>

---
### AnimateDiff
#### Paper: [AnimateDiff: Animate Your Personalized Text-to-Image Diffusion Models without Specific Tuning](https://arxiv.org/abs/2307.04725)
#### Code: [https://github.com/guoyww/AnimateDiff](https://github.com/guoyww/AnimateDiff)
![](https://github.com/guoyww/AnimateDiff/raw/main/__assets__/figs/adapter_explain.png)

---
### Stable Diffusion Video
#### Paper: [Stable Video Diffusion: Scaling Latent Video Diffusion Models to Large Datasets](https://arxiv.org/abs/2311.15127)
#### Code: [https://github.com/nateraw/stable-diffusion-videos](https://github.com/nateraw/stable-diffusion-videos)
![](https://huggingface.co/stabilityai/stable-video-diffusion-img2vid/resolve/main/output_tile.gif)

---
### [Animate Anyone](https://humanaigc.github.io/animate-anyone/)
#### Paper: [Animate Anyone: Consistent and Controllable Image-to-Video Synthesis for Character Animation](https://arxiv.org/abs/2311.17117)<br>
![](https://arxiv.org/html/2311.17117v3/x1.png)
![](https://arxiv.org/html/2311.17117v3/x2.png)

---
### [StyleCrafter](https://gongyeliu.github.io/StyleCrafter.github.io/)
#### Paper: [StyleCrafter: Enhancing Stylized Text-to-Video Generation with Style Adapter](https://arxiv.org/abs/2312.00330)
#### Code: [https://github.com/GongyeLiu/StyleCrafter](https://github.com/GongyeLiu/StyleCrafter)
![](https://github.com/GongyeLiu/StyleCrafter/blob/main/docs/showcase_1.gif?raw=true)
![](https://gongyeliu.github.io/StyleCrafter.github.io/pics/overview.png)
![](https://arxiv.org/html/2312.00330v2/x2.png)

---
### Sora
### Paper: [Sora: A Review on Background, Technology, Limitations, and Opportunities of Large Vision Models](https://arxiv.org/html/2402.17177v3)
![](https://arxiv.org/html/2402.17177v3/extracted/2402.17177v3/fig_yx/dit-uvit.png)

---
### [Outfit Anyone](https://humanaigc.github.io/outfit-anyone/)
#### Paper: [OutfitAnyone: Ultra-high Quality Virtual Try-On for Any Clothing and Any Person](https://arxiv.org/abs/2407.16224)
#### Code: [https://github.com/HumanAIGC/OutfitAnyone](https://github.com/HumanAIGC/OutfitAnyone)
![](https://humanaigc.github.io/outfit-anyone/content/images/framework/fm.jpg)
![](https://arxiv.org/html/2407.16224v1/extracted/5749086/fig/method/framework2.png)

---
### LTX-Video
#### Paper: [LTX-Video: Realtime Video Latent Diffusion](https://arxiv.org/abs/2501.00103)
![](https://arxiv.org/html/2501.00103v1/extracted/6102773/assets/figures/vae_encoder.png)
![](https://arxiv.org/html/2501.00103v1/extracted/6102773/assets/figures/transformer_architecture.png)

---
### Open-Sora
#### Paper: [Open-Sora 2.0: Training a Commercial-Level Video Generation Model in $200k](https://arxiv.org/abs/2503.09642)
#### Code: [https://github.com/hpcaitech/Open-Sora](https://github.com/hpcaitech/Open-Sora)
![](https://arxiv.org/html/2503.09642v1/x3.png)
![](https://arxiv.org/html/2503.09642v1/extracted/6273005/figs/open-sora-2.0-dit.png)

---
### Step-Video-TI2V
#### Paper: [Step-Video-TI2V Technical Report: A State-of-the-Art Text-Driven Image-to-Video Generation Model](https://arxiv.org/abs/2503.11251)
#### Code: [https://github.com/stepfun-ai/Step-Video-TI2V](https://github.com/stepfun-ai/Step-Video-TI2V)
![](https://arxiv.org/html/2503.11251v1/extracted/6280203/figure/ti2v-arch.png)

---
### WAN 2.2
#### Paper: [Wan: Open and Advanced Large-Scale Video Generative Models](https://arxiv.org/abs/2503.20314)
#### Code: [https://github.com/Wan-Video/Wan2.2](https://github.com/Wan-Video/Wan2.2)
#### [ComfyUI + WAN2.2](https://docs.comfy.org/tutorials/video/wan/wan2_2)

### Multi-Talk
#### Paper: [Let Them Talk: Audio-Driven Multi-Person Conversational Video Generation](https://arxiv.org/html/2505.22647v1)
#### Code: [https://github.com/MeiGen-AI/MultiTalk](https://github.com/MeiGen-AI/MultiTalk)
![](https://github.com/MeiGen-AI/MultiTalk/raw/main/assets/pipe.png)

---
### InfiniteTalk
#### Paper: [InfiniteTalk: Audio-driven Video Generation for Sparse-Frame Video Dubbing](https://arxiv.org/abs/2508.14033)
#### Code: [https://github.com/MeiGen-AI/InfiniteTalk](https://github.com/MeiGen-AI/InfiniteTalk)
![](https://github.com/MeiGen-AI/InfiniteTalk/raw/main/assets/pipeline.png)

---
### [Wan-S2V](https://humanaigc.github.io/wan-s2v-webpage/)
#### HuggingFace: [Wan-AI/Wan2.2-S2V-14B](https://huggingface.co/Wan-AI/Wan2.2-S2V-14B)
#### Paper: [Wan-S2V: Audio-Driven Cinematic Video Generation](https://arxiv.org/abs/2508.18621)

---
### UniVerse-1
#### Paper: [UniVerse-1: Unified Audio-Video Generation via Stitching of Experts](https://www.arxiv.org/abs/2509.06155)
#### Code: [https://github.com/Dorniwang/UniVerse-1-code/](https://github.com/Dorniwang/UniVerse-1-code/)
![](https://arxiv.org/html/2509.06155v1/x1.png)

---
### Wan-Animate
#### Paper: [Wan-Animate: Unified Character Animation and Replacement with Holistic Replication](https://arxiv.org/abs/2509.14055)
![](https://humanaigc.github.io/wan-animate/content/aa/arch.png)

---
### [VEO 3](https://aistudio.google.com/models/veo-3) 
#### Paper: [Video models are zero-shot learners and reasoners](https://arxiv.org/html/2509.20328v2)
<iframe width="790" height="444" src="https://www.youtube.com/embed/orcRl82lGLc" title="Veo 3.1 in the Gemini API" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### FlashVSR
#### Paper: [FlashVSR: Towards Real-Time Diffusion-Based Streaming Video Super-Resolution](https://arxiv.org/abs/2510.12747)
#### Code: [https://github.com/OpenImagingLab/FlashVSR](https://github.com/OpenImagingLab/FlashVSR)
![](https://github.com/OpenImagingLab/FlashVSR/raw/main/examples/WanVSR/assets/flowchart.jpg)

---
### TiDAR
#### [TiDAR: Think in Diffusion, Talk in Autoregression](https://arxiv.org/abs/2511.08923)
![](https://arxiv.org/html/2511.08923v1/x2.png)

---
### DiffusionVL
#### [DiffusionVL: Translating Any Autoregressive Models into Diffusion Vision Language Models](https://arxiv.org/abs/2512.15713)
![](https://arxiv.org/html/2512.15713v3/x2.png)
![](https://arxiv.org/html/2512.15713v3/x3.png)

---
### SRENDER
#### Paper: [Efficient Camera-Controlled Video Generation of Static Scenes via Sparse Diffusion and 3D Rendering](https://arxiv.org/abs/2601.09697)
![](https://arxiv.org/html/2601.09697v1/x1.png)
![](https://arxiv.org/html/2601.09697v1/x2.png)

---
### LTX-2
#### Paper: [LTX-2: Efficient Joint Audio-Visual Foundation Model](https://arxiv.org/abs/2601.03233)
![](https://arxiv.org/html/2601.03233v1/assets/figures/fig-1-overview-v2.png)

---
### daVinci-MagiHuman
#### Paper: [Speed by Simplicity: A Single-Stream Architecture for Fast Audio-Video Generative Foundation Model](https://arxiv.org/abs/2603.21986)
#### Code: [https://github.com/GAIR-NLP/daVinci-MagiHuman](https://github.com/GAIR-NLP/daVinci-MagiHuman)
![](https://arxiv.org/html/2603.21986v1/x1.png)
![](https://arxiv.org/html/2603.21986v1/figures/arch.png)

---
### [Runway](https://runwayml.com/)
#### [GWM-1](https://runwayml.com/research/introducing-runway-gwm-1)
#### [Gen-4.5](https://runwayml.com/research/introducing-runway-gen-4.5)

---
### [Kling](https://klingai.com/)
#### Paper: [Kling-MotionControl Technical Report](https://arxiv.org/abs/2603.03160)
![](https://arxiv.org/html/2603.03160v1/x1.png)
![](https://arxiv.org/html/2603.03160v1/x2.png)

---
### [SeedDance 2.0](https://seed.bytedance.com/en/?view_from=homepage_tab)
#### Paper: [Seedance 2.0: Advancing Video Generation for World Complexity](https://arxiv.org/abs/2604.14148)
<iframe width="1364" height="767" src="https://www.youtube.com/embed/BQXxywxTidU" title="Seedance 2.0 vs Kling 3.0 – The Results Shocked Me" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### [LTX-2.3](https://ltx.io/model/ltx-2-3)
#### Blog: [Lightricks 發布 LTX 2.3 開源影片生成模型，可在本地端製作 4K 50FPS 同步音訊 AI 影片](https://www.koc.com.tw/archives/633673)
* 首先，文字編碼器規模擴大 4 倍，大幅提升提示詞理解能力，能精確呈現攝影機運動、構圖和角色動作，讓生成結果更符合創作者的預期。
* 全新設計的 VAE（變分自編碼器）提供更清晰的細節和更穩定的運動畫質，有效改善前代作品常見的畫面模糊問題。也支援 Lora 可進行影片風格轉換功能。
* 圖像轉影片（I2V）功能從訓練階段即整合至模型架構中，顯著減少畫面停滯現象，並降低所謂的「肯納伯斯效應」（can nabs effect），使連續幀之間的過渡更加自然，而且也支援首尾幀功能與原生直橫格式影片生成。
* 音訊品質同步提升，是目前開源模型中少數支援音畫同時生成的本地端模型。新型 vocoder 降低背景雜音並強化音畫同步，解決過往 AI 生成的影片常見的音訊延遲或不同步問題。大家可以看看官方所釋出的宣傳影片，效果相當驚艷（以開源模型來說）
  
<iframe width="750" height="422" src="https://www.youtube.com/embed/o-7us-BR_gQ" title="LTX-2.3 Is Here: Sharper Detail, Native Portrait, Cleaner Audio" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### [JoyAI-Echo](https://echo-team-joy-future-academy-jd.github.io/Echo-LongVideo-Page/)
#### Code: [https://github.com/jd-opensource/JoyAI-Echo](https://github.com/jd-opensource/JoyAI-Echo)

---
## World Models

### Phantom
#### Paper: [Phantom: Physics-Infused Video Generation via Joint Modeling of Visual and Latent Physical Dynamics](https://arxiv.org/abs/2604.08503)
![](https://arxiv.org/html/2604.08503v1/x2.png)

---
### SANA-WM
#### Paper: [SANA-WM: Efficient Minute-Scale World Modeling with Hybrid Linear Diffusion Transformer](https://arxiv.org/abs/2605.15178)
#### Code: [https://github.com/NVlabs/Sana](https://github.com/NVlabs/Sana)
![](https://arxiv.org/html/2605.15178v1/x2.png)

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*


