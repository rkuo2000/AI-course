---
layout: post
title: RL for Robot Navigation
author: [Richard Kuo]
category: [Lecture]
tags: [jekyll, ai]
---

Introduction to Robot Navigation

---
## Humanoid

### Optimus Gen3
<iframe width="783" height="440" src="https://www.youtube.com/embed/kD3ehpBdUY4" title="Tesla’s NEW Optimus UPGRADE STUNS The ENTIRE INDUSTRY (GEN 3 Breakthrough)" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### Walker S2
<iframe width="783" height="440" src="https://www.youtube.com/embed/mHP1WGlw5Wk" title="Walker S2 - The World's First Humanoid Robot Capable of Autonomous Battery Swapping" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### Figure 03
<iframe width="783" height="440" src="https://www.youtube.com/embed/ybjhQF8ha90" title="特斯拉機器人殺手解說 2025 年 FIGURE 03 人形機器人的特徵" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### Figure 01
<iframe width="1169" height="658" src="https://www.youtube.com/embed/tpp8cykrauk" title="圖 01 OpenAI + 微軟的人工智能機器人更新令科技界震驚" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### ADAM (DeepMind's RoboTool)
**Paper:** [ADAM: a robotic companion for enhanced quality of life in aging populations](https://www.frontiersin.org/articles/10.3389/fnbot.2024.1337608/full)<br>
<iframe width="999" height="562" src="https://www.youtube.com/embed/bWg8qwCe4K0" title="新型模塊化人工智能機器人技術變得更加瘋狂（谷歌 DeepMind 的 RoboTool）" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
### NVIDIA Isaac GR00T N1
<iframe width="585" height="329" src="https://www.youtube.com/embed/m1CH-mgpdYg" title="NVIDIA Isaac GR00T N1: An Open Foundation Model for Humanoid Robots" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
## Simulated Environments

### Matterport3D
**Paper:** [Matterport3D: Learning from RGB-D Data in Indoor Environments](https://arxiv.org/abs/1709.06158)<br>
**Code:** [Matterport3D](https://github.com/niessner/Matterport)<br>

![](https://github.com/niessner/Matterport/blob/master/img/teaser.jpg?raw=true)

---
### Replica 
**Code:** [Replica Dataset](https://github.com/facebookresearch/Replica-Dataset)<br>
![](https://github.com/facebookresearch/Replica-Dataset/blob/main/assets/ReplicaModalities.png?raw=true)

---
### iGibson
**Paper:** [iGibson 2.0: Object-Centric Simulation for Robot Learning of Everyday Household Tasks](https://arxiv.org/abs/2108.03272)<br>
**Code:** [StanfordVL/iGibson](https://github.com/StanfordVL/iGibson)<br>
![](https://github.com/StanfordVL/iGibson/blob/master/docs/images/igibson.gif?raw=true)

---
### Habitat 2.0
**Paper:** [Habitat 2.0: Training Home Assistants to Rearrange their Habitat](https://arxiv.org/abs/2106.14405)<br>
**Code:** [facebookresearch/habitat-sim](https://github.com/facebookresearch/habitat-sim)<br>
<video controls>
  <source src="https://user-images.githubusercontent.com/2941091/126080914-36dc8045-01d4-4a68-8c2e-74d0bca1b9b8.mp4" type="video/mp4">
</video>

---
### Autonomous Indoor Robot Navigation
**Paper:** [Deep Reinforcement learning for real autonomous mobile robot navigation in indoor environments](https://arxiv.org/abs/2005.13857)<br>
**Code:** [](https://github.com/RoblabWh/RobLearn)<br>
<iframe width="742" height="417" src="https://www.youtube.com/embed/KyA2uTIQfxw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
![](https://d3i71xaburhd42.cloudfront.net/8a47843c2e664e5e7e218e2d891726d023619403/3-Figure4-1.png)

---
### DDPG 路徑規劃
**Blog:** [智慧送餐服務型機器人導航路徑之設計](https://www.phdbooks.com.tw/cn/magazine/detail/1225)<br>
路徑跟隨器有四個主軸：<br>
* 送餐路徑生成：從文件或上層發佈訊息獲取預先定義的路徑。
* 編輯航線路徑點：清除路徑中不合適的航線路徑點。
* MFAC無模型自適應控制之航段管制：自動調整送餐路徑之導航點之間的航段長度，依序共分成路徑跟隨之依據以及MFAC無模型自適應控制之應用。
* DWA之區域路徑傳遞：依照MFAC調整之結果，產出相關生成路徑，並以DWA進行區域設定。

* **自走車基於DDPG的室內路徑規劃**<br>
<iframe width="506" height="285" src="https://www.youtube.com/embed/TNRjb8q6XxM" title="自走車基於DDPG的室內路徑規劃" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### Long-Range Indoor Navigation
**Paper:** [Long-Range Indoor Navigation with PRM-RL](https://arxiv.org/abs/1902.09458)<br>
<iframe width="742" height="417" src="https://www.youtube.com/embed/xN-OWX5gKvQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
![](https://github.com/rkuo2000/AI-course/blob/gh-pages/images/Long-Range-Indoor-Navigation.png?raw=true)

---
### iSDF
**Arxiv**: [iSDF: Real-Time Neural Signed Distance Fields for Robot Perception](https://arxiv.org/abs/2204.02296)<br>
**Github**: [https://github.com/facebookresearch/iSDF](https://github.com/facebookresearch/iSDF)<br>
![](https://github.com/facebookresearch/iSDF/raw/main/.github/intro.gif)

---
### Tesla Vision-based ML model
**Patent**: [Vision-based machine learning model for autonomous driving with adjustable virtual camera](https://patents.google.com/patent/US20230057509A1/en)<br>
**Twitter**: [Tesla's Dual Network Vision System: The Core Technology Behind FSD v12.5](https://x.com/seti_park/status/1816021548345802862)<br>

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*


