---
layout: post # 指定文章佈局，通常是 post
title: Generative Speech
date: 2025-09-09 10:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [AIGC] # 文章標籤，您可以自訂
description: Text-to-Speech, Voice Cloning, Speech Seperation, ASR
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## Text-To-Speech (using TTS)

### [WaveNet](https://deepmind.com/blog/article/wavenet-generative-model-raw-audio)
#### Paper: [WaveNet: A Generative Model for Raw Audio](https://arxiv.org/abs/1609.03499)
![](https://lh3.googleusercontent.com/Zy5xK_i2F8sNH5tFtRa0SjbLp_CU7QwzS2iB5nf2ijIf_OYm-Q5D0SgoW9SmfbDF97tNEF7CmxaL-o6oLC8sGIrJ5HxWNk79dL1r7Rc=w1440-rw-v1)

#### Code: [https://github.com/r9y9/wavenet_vocoder](https://github.com/r9y9/wavenet_vocoder)
#### Colab: [Tacotron2_and_WaveNet_text_to_speech_demo.ipynb](https://colab.research.google.com/github/r9y9/Colaboratory/blob/master/Tacotron2_and_WaveNet_text_to_speech_demo.ipynb)

---
### Tacotron-2
#### Paper: [Natural TTS Synthesis by Conditioning WaveNet on Mel Spectrogram Predictions](https://arxiv.org/abs/1712.05884)
#### Code: [https://github.com/Rayhane-mamah/Tacotron-2](https://github.com/Rayhane-mamah/Tacotron-2)
![](https://camo.githubusercontent.com/d6c3e238b30a49a31c947dd0c5b344c452b53ab5eb735dc79675b67c92a2cf96/68747470733a2f2f707265766965772e6962622e636f2f625538734c532f5461636f74726f6e5f325f4172636869746563747572652e706e67)

#### Code: [Tacotron 2 (without wavenet)](https://github.com/NVIDIA/tacotron2)
![](https://github.com/NVIDIA/tacotron2/blob/master/tensorboard.png?raw=true)

---
### Few-shot Transformer TTS
#### Paper: [Multilingual Byte2Speech Models for Scalable Low-resource Speech Synthesis](https://arxiv.org/abs/2103.03541)
#### Code: [https://github.com/mutiann/few-shot-transformer-tts](https://github.com/mutiann/few-shot-transformer-tts)

---
### MetaAudio
#### Paper: [MetaAudio: A Few-Shot Audio Classification Benchmark](https://arxiv.org/abs/2204.02121)
#### Code: [MetaAudio-A-Few-Shot-Audio-Classification-Benchmark](https://github.com/CHeggan/MetaAudio-A-Few-Shot-Audio-Classification-Benchmark)
**Dataset:** ESC-50, NSynth, FSDKaggle18, BirdClef2020, VoxCeleb1

---
### SeamlessM4T
#### Paper: [SeamlessM4T: Massively Multilingual & Multimodal Machine Translation](https://arxiv.org/abs/2308.11596)
#### Code: [https://github.com/facebookresearch/seamless_communication](https://github.com/facebookresearch/seamless_communication)
#### Colab: [seamless_m4t_colab](https://github.com/camenduru/seamless-m4t-colab)

---
### Audiobox Aesthetics
#### Paper: [Meta Audiobox Aesthetics: Unified Automatic Quality Assessment for Speech, Music, and Sound]()
#### Code: [https://github.com/facebookresearch/audiobox-aesthetics](https://github.com/facebookresearch/audiobox-aesthetics)
<img width="50%" height="50%" src="https://github.com/facebookresearch/audiobox-aesthetics/raw/main/assets/aes_model.png">

---
### SV2TTS
#### Paper: [Transfer Learning from Speaker Verification to Multispeaker Text-To-Speech Synthesis](https://arxiv.org/abs/1806.04558)
#### Code: [CorentinJ/Real-Time-Voice-Cloning](https://github.com/CorentinJ/Real-Time-Voice-Cloning)

<iframe width="574" height="323" src="https://www.youtube.com/embed/-O_hYhToKoA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### Spark-TTS
#### Paper: [Spark-TTS: An Efficient LLM-Based Text-to-Speech Model with Single-Stream Decoupled Speech Tokens](https://arxiv.org/abs/2503.01710)
#### Code: [https://github.com/SparkAudio/Spark-TTS](https://github.com/SparkAudio/Spark-TTS)

* Inference Overview of Voice Cloning
![](https://github.com/SparkAudio/Spark-TTS/raw/main/src/figures/infer_voice_cloning.png)

* Inference Overview of Controlled Generation
![](https://github.com/SparkAudio/Spark-TTS/raw/main/src/figures/infer_control.png)

#### ComfyUI: [https://github.com/billwuhao/ComfyUI_SparkTTS](https://github.com/billwuhao/ComfyUI_SparkTTS)
#### Kaggle: [rkuo2000/Spark-TTS](https://www.kaggle.com/code/rkuo2000/spark-tts)

---
### IndexTTS2
#### Paper: [IndexTTS2: A Breakthrough in Emotionally Expressive and Duration-Controlled Auto-Regressive Zero-Shot Text-to-Speech](https://arxiv.org/abs/2506.21619)
![](https://arxiv.org/html/2506.21619v2/x1.png)
![](https://arxiv.org/html/2506.21619v2/x2.png)
#### Code: [https://github.com/index-tts/index-tts](https://github.com/index-tts/index-tts)

#### ComfyUI: [https://github.com/billwuhao/ComfyUI_IndexTTS](https://github.com/billwuhao/ComfyUI_IndexTTS)
#### Kaggle: [rkuo2000/Index-TTS2](https://www.kaggle.com/code/rkuo2000/index-tts2)

---
### VibeVoice
#### Paper: [VibeVoice Technical Report](https://arxiv.org/abs/2508.19205)
#### model: [microsoft/VibeVoice-1.5B](https://huggingface.co/microsoft/VibeVoice-1.5B)
#### Code: [https://github.com/microsoft/VibeVoice](https://github.com/microsoft/VibeVoice)
<img width="50%" height="50%" src="https://github.com/microsoft/VibeVoice/raw/main/Figures/MOS-preference.png">

#### ComfyUI: [https://github.com/Enemyx-net/VibeVoice-ComfyUI](https://github.com/Enemyx-net/VibeVoice-ComfyUI)

---
### FireRedTTS-2
#### Paper: [FireRedTTS-2: Towards Long Conversational Speech Generation for Podcast and Chatbot](https://arxiv.org/abs/2509.02020)
#### Code: [https://github.com/FireRedTeam/FireRedTTS2](https://github.com/FireRedTeam/FireRedTTS2)
![](https://arxiv.org/html/2509.02020v2/image/tts_model_framework.png)

#### ComfyUI: [https://github.com/1038lab/ComfyUI-FireRedTTS](https://github.com/1038lab/ComfyUI-FireRedTTS)

---
### VoxCPM
#### Paper: [VoxCPM: Tokenizer-Free TTS for Context-Aware Speech Generation and True-to-Life Voice Cloning](https://arxiv.org/abs/2509.24650)
![](https://arxiv.org/html/2509.24650v1/images/draft_1.png)

---
### [Qwen3-TTS](https://qwen.ai/blog?id=qwen3tts-0115)
#### Paper: [Qwen3-TTS Technical Report](https://arxiv.org/html/2601.15621v1)
#### Code: [https://github.com/QwenLM/Qwen3-TTS](https://github.com/QwenLM/Qwen3-TTS)
![](https://arxiv.org/html/2601.15621v1/figures/Tokenizer.png)
![](https://arxiv.org/html/2601.15621v1/figures/Qwen3TTS_1104.png)

---
### PersonaPlex
#### Paper: [PersonaPlex: Voice and Role Control for Full Duplex Conversational Speech Models](https://arxiv.org/abs/2602.06053)
#### Blog: [NVIDIA PersonaPlex：開源全雙工語音新紀元，打造零停頓的真正 AI 對話](https://tools.wingzero.tw/article/sn/3777)
#### Code: [https://github.com/NVIDIA/personaplex](https://github.com/NVIDIA/personaplex)
![](https://github.com/NVIDIA/personaplex/raw/main/assets/architecture_diagram.png)

---
### [VoxCPM2](https://openbmb.github.io/voxcpm2-demopage/)
#### Blog: [VoxCPM2 開源語音模型實測：清華團隊 20 億參數 TTS 在相似度基準上大幅領先 ElevenLabs](https://tenten.co/learning/voxcpm2-voice-ai-model/)
#### Code: [https://github.com/OpenBMB/VoxCPM](https://github.com/OpenBMB/VoxCPM)
![](https://github.com/OpenBMB/VoxCPM/raw/main/assets/voxcpm_model.png)

---
## Voice Cloning
**Paper**: [Voice Cloning: Comprehensive Survey](https://arxiv.org/abs/2505.00579)<br>
![](https://arxiv.org/html/2505.00579v1/x2.png)

---
### RVC-WebUI
#### Code: [https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI)

<iframe width="562" height="351" src="https://www.youtube.com/embed/1txQuGFEGQ0" title="真假分不清！最新版rvc变声器太牛了！实时变声，音色真实！无需训练，500+声音模型随便选！AI变声器分享！" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### AI 用你的聲音創建歌詞曲
<iframe width="994" height="491" src="https://www.youtube.com/embed/9nHbw0eUJeE" title="AI 用你的聲音創建歌詞曲 五音不全的人也可以靠AI實現當歌手的夢想 SunoAI + RVC WebUI + ChatGPT" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### GPT-SoVITS
#### Blog: [GPT-SoVITS 用 AI 快速複製你的聲音，搭配 Colab 免費入門](https://medium.com/dean-lin/gpt-sovits-%E7%94%A8-ai-%E5%BF%AB%E9%80%9F%E8%A4%87%E8%A3%BD%E4%BD%A0%E7%9A%84%E8%81%B2%E9%9F%B3-%E6%90%AD%E9%85%8D-colab-%E5%85%8D%E8%B2%BB%E5%85%A5%E9%96%80-f6a620cf7fc6)
#### Code: [https://github.com/RVC-Boss/GPT-SoVITS/](https://github.com/RVC-Boss/GPT-SoVITS/)
#### Kaggle: [rkuo2000/so-vits-svc-5-0](https://www.kaggle.com/code/rkuo2000/so-vits-svc-5-0)

---
### VITS SVC
Variational Inference with adversarial learning for end-to-end Singing Voice Conversion based on VITS<br>
#### Code: [https://github.com/PlayVoice/whisper-vits-svc](https://github.com/PlayVoice/whisper-vits-svc)

---
## Speech Seperation

### Looking to Listen
#### Paper: [Looking to Listen at the Cocktail Party: A Speaker-Independent Audio-Visual Model for Speech Separation](https://arxiv.org/abs/1804.03619)
#### Blog: [Looking to Listen: Audio-Visual Speech Separation](https://ai.googleblog.com/2018/04/looking-to-listen-audio-visual-speech.html)

![](https://3.bp.blogspot.com/-i8yGQmRfu6k/Ws03pWxgp2I/AAAAAAAACiM/3KgklbbHIvsYo4Tyw3N1TKa7Eywagr4eACLcBGAs/s640/image6.jpg)
<iframe width="640" height="360" src="https://www.youtube.com/embed/Z_ogAiVoE1g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="640" height="360" src="https://www.youtube.com/embed/uKwUL7vt03M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="640" height="360" src="https://www.youtube.com/embed/_7aMiqXubWo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### VoiceFilter
#### Paper: [VoiceFilter: Targeted Voice Separation by Speaker-Conditioned Spectrogram Masking](https://arxiv.org/abs/1810.04826)
#### Code: [https://github.com/maum-ai/voicefilter](https://github.com/maum-ai/voicefilter)
Training took about 20 hours on AWS p3.2xlarge(NVIDIA V100)<br>
![](https://github.com/maum-ai/voicefilter/raw/master/assets/voicefilter.png)

---
### VoiceFilter-Lite
#### Paper: [VoiceFilter-Lite: Streaming Targeted Voice Separation for On-Device Speech Recognition](https://arxiv.org/abs/2009.04323)
#### Blog: [](https://google.github.io/speaker-id/publications/VoiceFilter-Lite/)

![](https://google.github.io/speaker-id/publications/VoiceFilter-Lite/resources/architecture.png)
<iframe width="800" height="450" src="https://www.youtube.com/embed/BiWMZdnHuVs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
## Automatic Speech Recognition (ASR)

### [NeMO](https://github.com/NVIDIA/NeMo)
#### Paper: [NeMo: a toolkit for building AI applications using Neural Modules](https://arxiv.org/abs/1909.09577)
#### [Nemo ASR](https://catalog.ngc.nvidia.com/orgs/nvidia/collections/nemo_asr)<br>

### Whisper
#### Paper: [Robust Speech Recognition via Large-Scale Weak Supervision](https://arxiv.org/abs/2212.04356)
![](https://www.researchgate.net/profile/Zhanibek_Kozhirbayev/publication/376675691/figure/fig2/AS:11431281213642924@1703085158954/Whisper-architecture-representation.png)
#### Kaggle: [rkuo2000/asr-whisper](https://www.kaggle.com/code/rkuo2000/asr-whisper)

---
### Qwen-Audio
#### Paper: [Qwen-Audio: Advancing Universal Audio Understanding via Unified Large-Scale Audio-Language Models](https://arxiv.org/abs/2311.07919)
#### Code: [https://github.com/QwenLM/Qwen-Audio](https://github.com/QwenLM/Qwen-Audio)
![](https://github.com/QwenLM/Qwen-Audio/raw/main/assets/framework.png)

---
### [Faster-Whisper](https://github.com/SYSTRAN/faster-whisper)
faster-whisper is a reimplementation of OpenAI's Whisper model using CTranslate2, which is a fast inference engine for Transformer models.<br>
#### Kaggle: [rkuo2000/faster-whisper](https://www.kaggle.com/code/rkuo2000/faster-whisper)

---
### [Open Whisper-style Speech Models (OWSM)](https://www.wavlab.org/activities/2024/owsm/)
#### Paper: [OWSM v3.1: Better and Faster Open Whisper-Style Speech Models based on E-Branchformer](https://arxiv.org/abs/2401.16658)

---
### [Canary](https://huggingface.co/nvidia/canary-1b-v2)
#### Paper: [Less is More: Accurate Speech Recognition & Translation without Web-Scale Data](https://arxiv.org/abs/2406.19674)
#### Kaggle: [rkuo2000/asr-canary-1b](https://www.kaggle.com/code/rkuo2000/asr-canary-1b)

---
### [Whisper Large-v3](https://huggingface.co/openai/whisper-large-v3)
#### Kaggle: [rkuo2000/whisper-large-v3-turbo](https://www.kaggle.com/code/rkuo2000/whisper-large-v3-turbo)

---
### Omnilingual-ASR
#### Paper: [Omnilingual ASR: Open-Source Multilingual Speech Recognition for 1600+ Languages](https://ai.meta.com/research/publications/omnilingual-asr-open-source-multilingual-speech-recognition-for-1600-languages/)
#### Code: [https://github.com/facebookresearch/omnilingual-asr](https://github.com/facebookresearch/omnilingual-asr)

---
### [Granite-Speech](https://huggingface.co/ibm-granite/granite-speech-3.3-8b)
#### Paper: [Granite-speech: open-source speech-aware LLMs with strong English ASR capabilities](https://arxiv.org/abs/2505.08699)
![](https://arxiv.org/html/2505.08699v2/x1.png)

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*




