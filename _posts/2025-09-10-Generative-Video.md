---
layout: post # 指定文章佈局，通常是 post
title: Generative Video
date: 2025-09-10 10:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [AIGC] # 文章標籤，您可以自訂
description: Image-to-Video, Text-to-Video, Audio-to-Video
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## Image-to-Video

### Turn-A-Video
**Paper:** [Tune-A-Video: One-Shot Tuning of Image Diffusion Models for Text-to-Video Generation](https://arxiv.org/abs/2212.11565)<br>
**Code:** [https://github.com/showlab/Tune-A-Video](https://github.com/showlab/Tune-A-Video)<br>
<p align="center">
<img src="https://tuneavideo.github.io/assets/teaser.gif" width="1080px"/>  
<br>
<em>Given a video-text pair as input, our method, Tune-A-Video, fine-tunes a pre-trained text-to-image diffusion model for text-to-video generation.</em>
</p>

---
### Open-VCLIP
**Paper:** [Open-VCLIP: Transforming CLIP to an Open-vocabulary Video Model via Interpolated Weight Optimization](https://arxiv.org/abs/2302.00624)<br>
**Paper:** [Building an Open-Vocabulary Video CLIP Model with Better Architectures, Optimization and Data](https://arxiv.org/abs/2310.05010)<br>
**Code:** [https://github.com/wengzejia1/Open-VCLIP/](https://github.com/wengzejia1/Open-VCLIP/)<br>
![](https://github.com/wengzejia1/Open-VCLIP/blob/main/figures/firstpage.png?raw=true)

---
### [DyST](https://dyst-paper.github.io/)
**Paper:** [DyST: Towards Dynamic Neural Scene Representations on Real-World Videos]()<br>
<video controls><source src="https://dyst-paper.github.io/data/teaser.mp4" type="video/mp4"></video>
  
---
## Text-to-Motion

### TMR
**Paper:** [TMR: Text-to-Motion Retrieval Using Contrastive 3D Human Motion Synthesis](https://arxiv.org/abs/2305.00976)<br>
**Code:** [https://github.com/Mathux/TMR](https://github.com/Mathux/TMR)<br>

---
### Text-to-Motion Retrieval
**Paper:** [Text-to-Motion Retrieval: Towards Joint Understanding of Human Motion Data and Natural Language](https://arxiv.org/abs/2305.15842)<br>
**Code:** [https://github.com/mesnico/text-to-motion-retrieval](https://github.com/mesnico/text-to-motion-retrieval)<br>
`A person walks in a counterclockwise circle`<br>
![](https://github.com/mesnico/text-to-motion-retrieval/blob/main/teaser/example_74.gif?raw=true)
`A person is kneeling down on all four legs and begins to crawl`<br>
![](https://github.com/mesnico/text-to-motion-retrieval/raw/main/teaser/example_243.gif?raw=true)

---
### MotionDirector
**Paper:** [MotionDirector: Motion Customization of Text-to-Video Diffusion Models](https://arxiv.org/abs/2310.08465)<br>

---
### [GPT4Motion](https://gpt4motion.github.io/)
**Paper:** [GPT4Motion: Scripting Physical Motions in Text-to-Video Generation via Blender-Oriented GPT Planning](https://arxiv.org/abs/2311.12631)<br>
<video width="320" height="240" controls><src="https://gpt4motion.github.io/static/24videos/1.0_1.0_A%20basketball%20spins%20out%20of%20the%20air%20and%20falls.mp4" type="video/mp4">GPT4Motion BasketBall</video>

---
### Motion Editing
**Paper:** [Iterative Motion Editing with Natural Language](https://arxiv.org/abs/2312.11538)<br>

--- 
## Text-to-Video

### [Awesome Video Diffusion Models](https://github.com/ChenHsing/Awesome-Video-Diffusion-Models)

---
### Stable Diffusion Video
**Paper:** [Stable Video Diffusion: Scaling Latent Video Diffusion Models to Large Datasets](https://arxiv.org/abs/2311.15127)<br>
**Code:** [https://github.com/nateraw/stable-diffusion-videos](https://github.com/nateraw/stable-diffusion-videos)<br>
![](https://huggingface.co/stabilityai/stable-video-diffusion-img2vid/resolve/main/output_tile.gif)

---
### AnimateDiff
**Paper:** [AnimateDiff: Animate Your Personalized Text-to-Image Diffusion Models without Specific Tuning](https://arxiv.org/abs/2307.04725)<br>
**Paper:** [SparseCtrl: Adding Sparse Controls to Text-to-Video Diffusion Models](https://arxiv.org/abs/2311.16933)<br>
**Code:** [https://github.com/guoyww/AnimateDiff](https://github.com/guoyww/AnimateDiff)<br>
![](https://github.com/guoyww/AnimateDiff/raw/main/__assets__/figs/adapter_explain.png)

---
### Animate Anyone
**Paper:** [Animate Anyone: Consistent and Controllable Image-to-Video Synthesis for Character Animation](https://arxiv.org/abs/2311.17117)<br>

---
### StyleCrafter
**Paper:** [StyleCrafter: Enhancing Stylized Text-to-Video Generation with Style Adapter](https://arxiv.org/abs/2312.00330)<br>
**Code:** [https://github.com/GongyeLiu/StyleCrafter](https://github.com/GongyeLiu/StyleCrafter)<br>
![](https://github.com/GongyeLiu/StyleCrafter/blob/main/docs/showcase_1.gif?raw=true)

---
### [Outfit Anyone](https://humanaigc.github.io/outfit-anyone/)
**Code:** [https://github.com/HumanAIGC/OutfitAnyone](https://github.com/HumanAIGC/OutfitAnyone)<br>
<iframe width="1103" height="620" src="https://www.youtube.com/embed/jnNHcLdoxNk" title="Outfit Anyone + Animate Anyone" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
### [SignLLM](https://signllm.github.io/Prompt2Sign/)
**Paper:** [SignLLM: Sign Languages Production Large Language Models](https://arxiv.org/abs/2405.10718)<br>
**Code:** [https://github.com/SignLLM/Prompt2Sign](https://github.com/SignLLM/Prompt2Sign)<br>

---
### [AIF for Dynamic T2V](https://sites.google.com/view/aif-dynamic-t2v/)
**Paper**: [Improving Dynamic Object Interactions in Text-to-Video Generation with AI Feedback](https://arxiv.org/abs/2412.02617)<br>
![](https://arxiv.org/html/2412.02617v1/x2.png)


---
### VEO3
<iframe width="865" height="487" src="https://www.youtube.com/embed/pHWYdt78PwY" title="【超級簡單】2025最火爆AI影片神器！Google Veo3 普通人也能收割百萬流量😱" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### Flow
[Meet Flow: AI-powered filmmaking with Veo 3](https://blog.google/technology/ai/google-flow-veo-ai-filmmaking-tool/)<br>
<iframe width="1046" height="588" src="https://www.youtube.com/embed/A0VttaLy4sU" title="Introducing Flow | Google’s New AI Filmmaking Tool" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### Wan2.2
**Arxiv**: [Wan: Open and Advanced Large-Scale Video Generative Models](https://arxiv.org/abs/2503.20314)<br>
**Github**: [https://github.com/Wan-Video/Wan2.2](https://github.com/Wan-Video/Wan2.2)<br>

#### [ComfyUI + WAN2.2](https://docs.comfy.org/tutorials/video/wan/wan2_2)

---
### Wan-Animate
**HuggingFace:** [Wan-AI/Wan2.2-Animate-14B](https://huggingface.co/Wan-AI/Wan2.2-Animate-14B)<br>
**Arxiv**: [Wan-Animate: Unified Character Animation and Replacement with Holistic Replication](https://arxiv.org/abs/2509.14055)<br>
**Demo**: [https://huggingface.co/spaces/Wan-AI/Wan2.2-Animate](https://huggingface.co/spaces/Wan-AI/Wan2.2-Animate)<br>
![](https://humanaigc.github.io/wan-animate/content/aa/arch.png)

---
## Audio-to-Video

### Multi-Talk
**Paper**: [Let Them Talk: Audio-Driven Multi-Person Conversational Video Generation](https://arxiv.org/html/2505.22647v1)<br>
**Code**: [https://github.com/MeiGen-AI/MultiTalk](https://github.com/MeiGen-AI/MultiTalk)<br>
![](https://github.com/MeiGen-AI/MultiTalk/raw/main/assets/pipe.png)

---
### InfiniteTalk
**Paper**: [InfiniteTalk: Audio-driven Video Generation for Sparse-Frame Video Dubbing](https://arxiv.org/abs/2508.14033)<br>
**Code**: [https://github.com/MeiGen-AI/InfiniteTalk](https://github.com/MeiGen-AI/InfiniteTalk)<br>
![](https://github.com/MeiGen-AI/InfiniteTalk/raw/main/assets/pipeline.png)

---
### [Wan-S2V](https://humanaigc.github.io/wan-s2v-webpage/)
**HuggingFace**: [Wan-AI/Wan2.2-S2V-14B](https://huggingface.co/Wan-AI/Wan2.2-S2V-14B)<br>
**Arxiv**: [Wan-S2V: Audio-Driven Cinematic Video Generation](https://arxiv.org/abs/2508.18621)<br>
**Demo**: [https://huggingface.co/spaces/Wan-AI/Wan2.2-S2V](https://huggingface.co/spaces/Wan-AI/Wan2.2-S2V)<br>

---
### UniVerse-1
**Paper**: [UniVerse-1: Unified Audio-Video Generation via Stitching of Experts](https://www.arxiv.org/abs/2509.06155)<br>
![](https://arxiv.org/html/2509.06155v1/x1.png)
**Code**: [https://github.com/Dorniwang/UniVerse-1-code/](https://github.com/Dorniwang/UniVerse-1-code/)<br>

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*

