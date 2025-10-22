---
layout: post # 指定文章佈局，通常是 post
title: Generative Song
date: 2025-09-10 08:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [AIGC] # 文章標籤，您可以自訂
description: Text-to-Music, Text-to-Song
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## Text to Music

### [MusicLM](https://google-research.github.io/seanet/musiclm/examples/) 
**Paper**: [MusicLM: Generating Music From Text](https://arxiv.org/abs/2301.11325)<br>
**Code**: [https://github.com/lucidrains/musiclm-pytorch](https://github.com/lucidrains/musiclm-pytorch)<br>
**Code**: [https://github.com/zhvng/open-musiclm](https://github.com/zhvng/open-musiclm)<br>
![](https://github.com/zhvng/open-musiclm/raw/main/musiclm.png)

---
### [AudioCraft](https://ai.meta.com/resources/models-and-libraries/audiocraft/)
**Paper**: [Simple and Controllable Music Generation](https://arxiv.org/abs/2306.05284)<br>
**Code**: [https://github.com/facebookresearch/audiocraft](https://github.com/facebookresearch/audiocraft)<br>
![](https://miro.medium.com/v2/resize:fit:720/format:webp/0*Zka1L3btnQbmyZwK)

---
### LLM2Vec
**Paper**: [LLM2Vec: Large Language Models Are Secretly Powerful Text Encoders](https://arxiv.org/abs/2404.05961)<br>

---
### Yue
**Paper**: [YuE: Scaling Open Foundation Models for Long-Form Music Generation](https://arxiv.org/abs/2404.05961)<br>
![](https://arxiv.org/html/2503.08638v2/x1.png)

---
### Instruct-MusicGen
**Paper**: [Instruct-MusicGen: Unlocking Text-to-Music Editing for Music Language Models via Instruction Tuning](https://arxiv.org/abs/2405.18386)<br>
**Code**: [https://github.com/ldzhangyx/instruct-MusicGen](https://github.com/ldzhangyx/instruct-MusicGen)<br>
**Demo**: [https://bit.ly/instruct-musicgen](https://bit.ly/instruct-musicgen)<br>
<img width="50%" height="50%" src="https://arxiv.org/html/2405.18386v3/x2.png">

---
### [Stable Audio Open](https://stability.ai/news/stable-audio-open-research-paper)
**Paper**: [Stable Audio Open](https://arxiv.org/abs/2407.14358)<br>
**Code**: [https://github.com/Stability-AI/stable-audio-tools](https://github.com/Stability-AI/stable-audio-tools)<br>

---
### Seed-Music
**Paper**: [Seed-Music: A Unified Framework for High Quality and Controlled Music Generation](https://arxiv.org/html/2409.09214v3)<br>
![](https://arxiv.org/html/2409.09214v3/x2.png)

---
## Text to Song

### SongCreator 
**Paper**: [SongCreator: Lyrics-based Universal Song Generation](https://arxiv.org/abs/2409.06029)<br>
![](https://arxiv.org/html/2409.06029v2/x1.png)

#### Dual-sequence language model (DSLM)
The DSLM can utilize specific attention mask strategy to achieve different song generation tasks. <br>
![](https://arxiv.org/html/2409.06029v2/x2.png)

---
### SongGen
**Paper**: [SongGen: A Single Stage Auto-regressive Transformer for Text-to-Song Generation](https://arxiv.org/html/2502.13128v2)<br>
**Code**: [https://github.com/LiuZH-19/SongGen](https://github.com/LiuZH-19/SongGen)<br>

---
### DiffRhythm
**Paper**: [DiffRhythm: Blazingly Fast and Embarrassingly Simple End-to-End Full-Length Song Generation with Latent Diffusion](https://arxiv.org/html/2503.01183v1)<br>
**Code**: [https://github.com/ASLP-lab/DiffRhythm](https://github.com/ASLP-lab/DiffRhythm)<br>
![](https://github.com/ASLP-lab/DiffRhythm/raw/main/src/diffrhythm.jpg)

---
### DiffRhythm+
**Paper**: [DiffRhythm+: Controllable and Flexible Full-Length Song Generation with Preference Optimization](https://arxiv.org/html/2507.12890v2)<br>
![](https://arxiv.org/html/2507.12890v2/x1.png)

#### [ComfyUI DiffRhythm](https://github.com/billwuhao/ComfyUI_DiffRhythm)
![](https://github.com/billwuhao/ComfyUI_DiffRhythm/blob/master/images/2025-05-13_01-51-00.png?raw=true)

---
### JAM
**Paper**: [JAM: A Tiny Flow-based Song Generator with Fine-grained Controllability and Aesthetic Alignment](https://arxiv.org/html/2507.20880v1)<br>
**Code**: [https://github.com/declare-lab/jamify](https://github.com/declare-lab/jamify)<br>
![](https://github.com/declare-lab/jamify/raw/main/jam-teaser.png)

![](https://github.com/declare-lab/jamify/raw/main/jam.png)

---
### [ACE-Step](https://ace-step.github.io/)
**Paper**: [ACE-Step: A Step Towards Music Generation Foundation Model](https://arxiv.org/html/2506.00045v1)<br>
**Code**: [https://github.com/ace-step/ACE-Step](https://github.com/ace-step/ACE-Step)<br>
![](https://ace-step.github.io/raw/fig/ACE-Step_framework.png)

**ComfyUI**: [https://github.com/billwuhao/ComfyUI_ACE-Step](https://github.com/billwuhao/ComfyUI_ACE-Step)<br>
![](https://github.com/billwuhao/ComfyUI_ACE-Step/raw/main/images/2025-05-14_14-23-50.png)

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*




