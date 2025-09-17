---
layout: post
title: Generative Speech 
author: [Richard Kuo]
category: [Lecture]
tags: [jekyll, ai]
---

Introduction to Text-To-Speech, Voice Cloning, Voice Conversion, Automatic Speech Recognition(ASR).

---
## Text-To-Speech (using TTS)

### WaveNet
**Paper:** [WaveNet: A Generative Model for Raw Audio](https://arxiv.org/abs/1609.03499)<br>
**Code:** [r9y9/wavenet_vocoder](https://github.com/r9y9/wavenet_vocoder)<br>
With a pre-trained model provided here, you can synthesize waveform given a mel spectrogram, not raw text.<br>
You will need mel-spectrogram prediction model (such as Tacotron2) to use the pre-trained models for TTS.<br>
**Demo:** [An open source implementation of WaveNet vocoder](https://r9y9.github.io/wavenet_vocoder/)<br>
**Blog:** [WaveNet: A generative model for raw audio](https://deepmind.com/blog/article/wavenet-generative-model-raw-audio)<br>
![](https://lh3.googleusercontent.com/Zy5xK_i2F8sNH5tFtRa0SjbLp_CU7QwzS2iB5nf2ijIf_OYm-Q5D0SgoW9SmfbDF97tNEF7CmxaL-o6oLC8sGIrJ5HxWNk79dL1r7Rc=w1440-rw-v1)

---
### Tacotron-2
**Paper:** [Natural TTS Synthesis by Conditioning WaveNet on Mel Spectrogram Predictions](https://arxiv.org/abs/1712.05884)<br>
**Code:** [Rayhane-mamah/Tacotron-2](https://github.com/Rayhane-mamah/Tacotron-2)<br>
![](https://camo.githubusercontent.com/d6c3e238b30a49a31c947dd0c5b344c452b53ab5eb735dc79675b67c92a2cf96/68747470733a2f2f707265766965772e6962622e636f2f625538734c532f5461636f74726f6e5f325f4172636869746563747572652e706e67)

**Code:** [Tacotron 2 (without wavenet)](https://github.com/NVIDIA/tacotron2)<br>
![](https://github.com/NVIDIA/tacotron2/blob/master/tensorboard.png?raw=true)

---
### Few-shot Transformer TTS
**Paper:** [Multilingual Byte2Speech Models for Scalable Low-resource Speech Synthesis](https://arxiv.org/abs/2103.03541)<br>
**Code:** [https://github.com/mutiann/few-shot-transformer-tts](https://github.com/mutiann/few-shot-transformer-tts)<br>

---
### MetaAudio
**Paper:** [MetaAudio: A Few-Shot Audio Classification Benchmark](https://arxiv.org/abs/2204.02121)<br>
**Code:** [MetaAudio-A-Few-Shot-Audio-Classification-Benchmark](https://github.com/CHeggan/MetaAudio-A-Few-Shot-Audio-Classification-Benchmark)<br>
**Dataset:** ESC-50, NSynth, FSDKaggle18, BirdClef2020, VoxCeleb1

---
### SeamlessM4T
**Paper:** [SeamlessM4T: Massively Multilingual & Multimodal Machine Translation](https://arxiv.org/abs/2308.11596)<br>
**Code:** [https://github.com/facebookresearch/seamless_communication](https://github.com/facebookresearch/seamless_communication)<br>
**Colab:** [seamless_m4t_colab](https://github.com/camenduru/seamless-m4t-colab)<br>
[app.py](https://huggingface.co/spaces/facebook/seamless_m4t/blob/main/app.py)<br>

---
### Stable-TTS
**Paper**: [Stable-TTS: Stable Speaker-Adaptive Text-to-Speech Synthesis via Prosody Prompting]()<br>
![](https://arxiv.org/html/2412.20155v1/x2.png)
**Demo**: [https://huggingface.co/spaces/KdaiP/StableTTS1.1](https://huggingface.co/spaces/KdaiP/StableTTS1.1)<br>

---
### Audiobox Aesthetics
**Paper**: [Meta Audiobox Aesthetics: Unified Automatic Quality Assessment for Speech, Music, and Sound]()<br>
**Github**: [https://github.com/facebookresearch/audiobox-aesthetics](https://github.com/facebookresearch/audiobox-aesthetics)<br>
![](https://github.com/facebookresearch/audiobox-aesthetics/raw/main/assets/aes_model.png)

---
### Spark-TTS
**Paper**: [Spark-TTS: An Efficient LLM-Based Text-to-Speech Model with Single-Stream Decoupled Speech Tokens](https://arxiv.org/abs/2503.01710)<br>
**Github**: [https://github.com/SparkAudio/Spark-TTS](https://github.com/SparkAudio/Spark-TTS)<br>

**Inference Overview of Voice Cloning** <br>
![](https://github.com/SparkAudio/Spark-TTS/raw/main/src/figures/infer_voice_cloning.png)
**Inference Overview of Controlled Generation** <br>
![](https://github.com/SparkAudio/Spark-TTS/raw/main/src/figures/infer_control.png)

**Kaggle**: [https://www.kaggle.com/code/rkuo2000/spark-tts](https://www.kaggle.com/code/rkuo2000/spark-tts)<br>

---
### Index-TTS
**Paper**: [IndexTTS2: A Breakthrough in Emotionally Expressive and Duration-Controlled Auto-Regressive Zero-Shot Text-to-Speech](https://arxiv.org/abs/2506.21619)<br>
![](https://arxiv.org/html/2506.21619v2/x1.png)
![](https://arxiv.org/html/2506.21619v2/x2.png)
**Paper**: [IndexTTS: An Industrial-Level Controllable and Efficient Zero-Shot Text-To-Speech System](https://arxiv.org/abs/2502.05512)<br>
**Github**: [https://github.com/index-tts/index-tts](https://github.com/index-tts/index-tts)<br>
![](https://github.com/index-tts/index-tts/raw/main/assets/IndexTTS2.png)

---
### FireRedTTS-2
**Paper**: [FireRedTTS-2: Towards Long Conversational Speech Generation for Podcast and Chatbot](https://arxiv.org/abs/2509.02020)<br>
**HuggingFace**: [FireRedTeam/FireRedTTS2https](https://huggingface.co/FireRedTeam/FireRedTTS2)
**Github**: [https://github.com/FireRedTeam/FireRedTTS2](https://github.com/FireRedTeam/FireRedTTS2)<br>
FireRedTTS‑2 is a long-form streaming TTS system for multi-speaker dialogue generation, delivering stable, natural speech with reliable speaker switching and context-aware prosody<br>
* Long Conversational Speech Generation
* Multilingual Support
* Ultra-Low Latency (on an L20 GPU, our first-packet latency as low as 140ms)
* Strong Stability
* Random Timbre Generation
  
---
## Voice Conversion
**Paper:** [An Overview of Voice Conversion and its Challenges: From Statistical Modeling to Deep Learning](https://arxiv.org/abs/2008.03648)<br>
![](https://d3i71xaburhd42.cloudfront.net/4e1f36855442b761729dad4507513e23ca66206c/7-Figure2-1.png)

**Blog:** [Voice Cloning Using Deep Learning](https://medium.com/the-research-nest/voice-cloning-using-deep-learning-166f1b8d8595)<br>

---
### Voice Cloning
**Paper:** [Voice Cloning: Comprehensive Survey](https://arxiv.org/abs/2505.00579)<br>
![](https://arxiv.org/html/2505.00579v1/x3.png)
![](https://arxiv.org/html/2505.00579v1/x2.png)

---
### SV2TTS
**Blog:** [Voice Cloning: Corentin's Improvisation On SV2TTS](https://www.datasciencecentral.com/profiles/blogs/voice-cloning-corentin-s-improvisation-on-sv2tts)<br>
**Paper:** [Transfer Learning from Speaker Verification to Multispeaker Text-To-Speech Synthesis](https://arxiv.org/abs/1806.04558)<br>
**Code:** [CorentinJ/Real-Time-Voice-Cloning](https://github.com/CorentinJ/Real-Time-Voice-Cloning)<br>

![](https://storage.ning.com/topology/rest/1.0/file/get/8569870256)

**Synthesizer** : The synthesizer is Tacotron2 without Wavenet<br>
![](https://storage.ning.com/topology/rest/1.0/file/get/8569881687)

**SV2TTS Toolbox**<br>
<iframe width="1148" height="646" src="https://www.youtube.com/embed/-O_hYhToKoA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### [NeMO](https://github.com/NVIDIA/NeMo)
[Nemo ASR](https://catalog.ngc.nvidia.com/orgs/nvidia/collections/nemo_asr)<br>
[Automatic Speech Recognition (ASR)](https://docs.nvidia.com/deeplearning/nemo/user-guide/docs/en/main/asr/intro.html)<br>

---
### RVC vs SoftVC
"Retrieval-based Voice Conversion" 和 "SoftVC VITS Singing Voice Conversion" 是兩種聲音轉換技術的不同變種。以下是它們之間的一些區別：<br>

1.方法原理：<br>
Retrieval-based Voice Conversion：這種方法通常涉及使用大規模的語音資料庫或語音庫，從中檢索與輸入語音相似的聲音樣本，並將輸入語音轉換成與檢索到的聲音樣本相似的聲音。它使用檢索到的聲音作為目標來進行聲音轉換。<br>
SoftVC VITS Singing Voice Conversion：這是一種基於神經網路的聲音轉換方法，通常使用變分自動編碼器（Variational Autoencoder，VAE）或其他神經網路架構。專注於歌聲轉換，它的目標是將輸入歌聲樣本轉換成具有不同特徵的歌聲，例如性別、音調等。<br>

2.應用領域：<br>
Retrieval-based Voice Conversion 通常用於語音轉換任務，例如將一個人的語音轉換成另一個人的語音。它也可以用於歌聲轉換，但在歌聲轉換方面通常不如專門設計的方法表現出色。<br>
SoftVC VITS Singing Voice Conversion 主要用於歌聲轉換任務，特別是針對歌手之間的音樂聲音特徵轉換，例如將男性歌手的聲音轉換成女性歌手的聲音，或者改變歌曲的音調和音樂特徵。<br>

3.技術複雜性：<br>
Retrieval-based Voice Conversion 的實現通常較為簡單，因為它主要依賴於聲音樣本的檢索和聲音特徵的映射。<br>
SoftVC VITS Singing Voice Conversion 更複雜，因為它需要訓練深度神經網路模型，可能需要大量的數據和計算資源。<br>

---
### Retrieval-based Voice Conversion
**Blog:** [RVC-WebUI開源專案教學](https://gogoplus.net/%E7%BF%BB%E5%94%B1%E6%9C%80%E5%A5%BD%E7%94%A8%E7%9A%84%E9%96%8B%E6%BA%90%E7%A8%8B%E5%BC%8F-rvc-webui-%E5%85%8B%E9%9A%86%E4%BD%A0%E7%9A%84%E8%81%B2%E9%9F%B3/)<br>
**Code:** [https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI](https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI)<br>

<iframe width="994" height="491" src="https://www.youtube.com/embed/9nHbw0eUJeE" title="AI 用你的聲音創建歌詞曲 五音不全的人也可以靠AI實現當歌手的夢想 SunoAI + RVC WebUI + ChatGPT" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### GPT-SoVITS
**Blog:** [GPT-SoVITS 用 AI 快速複製你的聲音，搭配 Colab 免費入門](https://medium.com/dean-lin/gpt-sovits-%E7%94%A8-ai-%E5%BF%AB%E9%80%9F%E8%A4%87%E8%A3%BD%E4%BD%A0%E7%9A%84%E8%81%B2%E9%9F%B3-%E6%90%AD%E9%85%8D-colab-%E5%85%8D%E8%B2%BB%E5%85%A5%E9%96%80-f6a620cf7fc6)<br>
**Code:** [https://github.com/RVC-Boss/GPT-SoVITS/](https://github.com/RVC-Boss/GPT-SoVITS/)<br>
**Kaggle:** [https://www.kaggle.com/code/rkuo2000/so-vits-svc-5-0](https://www.kaggle.com/code/rkuo2000/so-vits-svc-5-0)<br>

---
### VITS SVC
Variational Inference with adversarial learning for end-to-end Singing Voice Conversion based on VITS<br>
**Github**: [https://github.com/PlayVoice/whisper-vits-svc](https://github.com/PlayVoice/whisper-vits-svc)<br>

---
### BreezyVoice
**Paper:** [BreezyVoice: Adapting TTS for Taiwanese Mandarin with Enhanced Polyphone Disambiguation -- Challenges and Insights](https://arxiv.org/abs/2501.17790)<br>
**Code:** [https://github.com/mtkresearch/BreezyVoice](https://github.com/mtkresearch/BreezyVoice)<br>
![](https://raw.githubusercontent.com/mtkresearch/BreezyVoice/main/images/flowchart.png)

---
## Speech Seperation

### Looking to Listen
**Paper:** [Looking to Listen at the Cocktail Party: A Speaker-Independent Audio-Visual Model for Speech Separation](https://arxiv.org/abs/1804.03619)<br>
**Blog:** [Looking to Listen: Audio-Visual Speech Separation](https://ai.googleblog.com/2018/04/looking-to-listen-audio-visual-speech.html)<br>

![](https://3.bp.blogspot.com/-i8yGQmRfu6k/Ws03pWxgp2I/AAAAAAAACiM/3KgklbbHIvsYo4Tyw3N1TKa7Eywagr4eACLcBGAs/s640/image6.jpg)
<iframe width="640" height="360" src="https://www.youtube.com/embed/Z_ogAiVoE1g" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="640" height="360" src="https://www.youtube.com/embed/uKwUL7vt03M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<iframe width="640" height="360" src="https://www.youtube.com/embed/_7aMiqXubWo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
### VoiceFilter
**Paper:** [VoiceFilter: Targeted Voice Separation by Speaker-Conditioned Spectrogram Masking](https://arxiv.org/abs/1810.04826)<br>
**Github**: [https://github.com/maum-ai/voicefilter](https://github.com/maum-ai/voicefilter)<br>
Training took about 20 hours on AWS p3.2xlarge(NVIDIA V100)<br>
![](https://github.com/maum-ai/voicefilter/raw/master/assets/voicefilter.png)

---
### VoiceFilter-Lite
**Paper:** [VoiceFilter-Lite: Streaming Targeted Voice Separation for On-Device Speech Recognition](https://arxiv.org/abs/2009.04323)<br>
**Blog:** [](https://google.github.io/speaker-id/publications/VoiceFilter-Lite/)<br>

![](https://google.github.io/speaker-id/publications/VoiceFilter-Lite/resources/architecture.png)
<iframe width="800" height="450" src="https://www.youtube.com/embed/BiWMZdnHuVs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---
## Automatic Speech Recognition (ASR)

### Whisper
**Paper:** [Robust Speech Recognition via Large-Scale Weak Supervision](https://arxiv.org/abs/2212.04356)<br>
![](https://www.researchgate.net/profile/Zhanibek_Kozhirbayev/publication/376675691/figure/fig2/AS:11431281213642924@1703085158954/Whisper-architecture-representation.png)
**Kaggle:** [https://www.kaggle.com/code/rkuo2000/whisper](https://www.kaggle.com/code/rkuo2000/whisper)<br>

---
### [Faster-Whisper](https://github.com/SYSTRAN/faster-whisper)
faster-whisper is a reimplementation of OpenAI's Whisper model using CTranslate2, which is a fast inference engine for Transformer models.<br>
**Kaggle:** [https://www.kaggle.com/code/rkuo2000/faster-whisper](https://www.kaggle.com/code/rkuo2000/faster-whisper)<br>

---
### [Open Whisper-style Speech Models (OWSM)](https://www.wavlab.org/activities/2024/owsm/)
**Paper:** [OWSM v3.1: Better and Faster Open Whisper-Style Speech Models based on E-Branchformer](https://arxiv.org/abs/2401.16658)<br>

---
### Qwen-Audio
**Github:** [https://github.com/QwenLM/Qwen-Audio](https://github.com/QwenLM/Qwen-Audio)<br>
![](https://github.com/QwenLM/Qwen-Audio/raw/main/assets/framework.png)

---
### Meta SpiritLM
**Paper**: [Spirit LM: Interleaved Spoken and Written Language Model](https://arxiv.org/abs/2402.05755)
**Blog**: [Meta開源首個多模態語言模型Meta Spirit LM](https://www.ithome.com.tw/news/165587)<br>
**Github**: [https://github.com/facebookresearch/spiritlm](https://github.com/facebookresearch/spiritlm)<br>
![](https://github.com/facebookresearch/spiritlm/raw/main/assets/spiritlm_overview.png)

---
### Canary
**model:** [nvidia/canary-1b](https://huggingface.co/nvidia/canary-1b)<br>
**Paper:** [Less is More: Accurate Speech Recognition & Translation without Web-Scale Data](https://arxiv.org/abs/2406.19674)<br>

---
### [Whisper Large-v3](https://huggingface.co/openai/whisper-large-v3)
**model:** openai/whisper-large-v3<br>
**model:** openai/whisper-large-v3-turbo<br>
**Kaggle:** [https://www.kaggle.com/code/rkuo2000/whisper-large-v3-turbo](https://www.kaggle.com/code/rkuo2000/whisper-large-v3-turbo)<br>

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*



