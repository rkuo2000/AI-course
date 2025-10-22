---
layout: post # 指定文章佈局，通常是 post
title: Generative Image
date: 2025-09-11 08:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [AIGC] # 文章標籤，您可以自訂
description: Text-to-Image, Text-to-3D, Image-to-3D
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## Text-to-Image
**News:** [An A.I.-Generated Picture Won an Art Prize. Artists Aren’t Happy.](https://www.nytimes.com/2022/09/02/technology/ai-artificial-intelligence-artists.html)<br>
![](https://static01.nyt.com/images/2022/09/01/business/00roose-1/merlin_212276709_3104aef5-3dc4-4288-bb44-9e5624db0b37-superJumbo.jpg?quality=75&auto=webp)

---
### Diffusion Models
**Paper:** [High-Resolution Image Synthesis with Latent Diffusion Models](https://arxiv.org/abs/2112.10752)<br>
![](https://miro.medium.com/v2/resize:fit:720/format:webp/0*rW_y1kjruoT9BSO0.png)

**Blog:** [Introduction to Diffusion Models for Machine Learning](https://www.assemblyai.com/blog/diffusion-models-for-machine-learning-introduction/)<br>

Diffusion Models are a method of creating data that is similar to a set of training data. <br>
They train by destroying the training data through the addition of noise, and then learning to recover the data by reversing this noising process. Given an input image, the Diffusion Model will iteratively corrupt the image with Gaussian noise in a series of timesteps, ultimately leaving pure Gaussian noise, or "TV static".
![](https://www.assemblyai.com/blog/content/images/size/w1000/2022/06/image-5.png)
The Diffusion Model will then work backwards, learning how to isolate and remove the noise at each timestep, undoing the destruction process that just occurred.<br>
Once trained, the model can then be "split in half", and we can start from randomly sampled Gaussian noise which we use the Diffusion Model to gradually denoise in order to generate an image.
![](https://www.assemblyai.com/blog/content/images/size/w1000/2022/06/image-4.png)

---
### [Midjourney](https://www.midjourney.com/)
**[Model Versions](https://docs.midjourney.com/docs/model-versions)** <br>
Version 6.1 was released on July 30, 2024 as the new default model. It produces more coherent images with more precise details and textures, and generates images approximately 25% faster than Version 6.<br>
<p>
<img width="50%" height="50%" src="https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/poppies-v6-1.png">
<img width="50%" height="50%" src="https://cdn.document360.io/3040c2b6-fead-4744-a3a9-d56d621c6c7e/Images/Documentation/collage-v6-1.png">
</p>

* **Forward Diffusion Process:** The diffusion model starts by taking an input image and gradually adding Gaussian noise.

* **Noise Accumulation:** The model continues to add more noise to the image. After each addition, randomized image sections are covered in noise until the original image is transformed into a noisy or grain-covered version. More noise will result in a more different generation, while less will produce a more similar generation to the original image.

* **Denoising Process:** After adding the desired amount of noise, which Midjourney users can partially control with prompt weighting, the model learns to recover the original image by reversing the noising process.

* **Iterative Refinement:** Denoising is performed iteratively, gradually reducing the noise level in the image. At each step, the diffusion model improves the image’s quality and ability to refine over time.

* **Training and Predictive Learning:** The steps above repeat for as many images in the training dataset as possible. The model eventually learns to predict the original image from the noisy image.

* **Generating New Data:** Once the model is trained, it creates new images by passing random noise samples and generating the colors and shapes from the patterns the model picked up during training. This creates unique images similar to the training data but slightly different, resulting in various possible outputs.

---
### [DALL.E, E2, and storyDALL-E](https://zhangtemplar.github.io/dalle/)

### [DALL.E](https://openai.com/blog/dall-e/)
DALL·E is a 12-billion parameter version of GPT-3 trained to generate images from text descriptions, using a dataset of text–image pairs. <br>
**Paper:** [Zero-Shot Text-to-Image Generation](https://arxiv.org/abs/2102.12092)<br> 
**Code:** [openai/DALL-E](https://github.com/openai/DALL-E)<br>
The overview of DALL-E could be illustrated as below. It contains two components: for image, VQGAN (vector quantized GAN) is used to map the 256x256 image to a 32x32 grid of image token and each token has 8192 possible values; then this token is combined with 256 BPE=encoded text token is fed into to train the autoregressive transformer. The text token is set to 256 by maximal.
<p><img width="50%" height="50%" src="https://raw.githubusercontent.com/zhangtemplar/zhangtemplar.github.io/master/uPic/2022_09_30_16_08_31_105325789-46d94700-5bcd-11eb-9c91-818e8b5d6a35.jpeg"></p>

---
### [DALL.E-2](https://openai.com/dall-e-2/)
**Paper:** [Hierarchical Text-Conditional Image Generation with CLIP Latents](https://arxiv.org/abs/2204.06125)<br>
![](https://pic3.zhimg.com/80/v2-e096e3cf8a1e7a9f569b18f658da574e_720w.jpg)

---
### [How Does DALL·E 2 Work?](https://medium.com/augmented-startups/how-does-dall-e-2-work-e6d492a2667f)
Compared to DALL·E’s 12-billion parameters, DALL·E 2 works on a 3.5-billion parameter model and another 1.5-billion parameter model to enhance the resolution of its images.

**DALL·E 2 image generation process** <br>
![](https://miro.medium.com/v2/resize:fit:720/format:webp/1*w2W7tw7LtDOvToKNPE34lw.png)

**CLIP Training** <br>
![](https://miro.medium.com/v2/resize:fit:720/format:webp/1*I0VlIbh5eMXBQ2UysUvmSA.gif)

**Diffusion Models** <br>
![](https://miro.medium.com/v2/resize:fit:720/format:webp/1*bcpdCHJOmQ_05rbq_EIYCg.gif)
Diffusion models are transformer-based generative models. They take a piece of data, for example, a photo, and gradually add noise over timesteps, until it is not recognizable. And from that point, they try to reconstruct the image to its original form. In doing so, they learn how to generate images or any other kind of data.

---
### [LAION-5B Dataset](https://laion.ai/blog/laion-5b/)
5.85 billion CLIP-filtered image-text pairs<br>
**Paper:** [LAION-5B: An open large-scale dataset for training next generation image-text models](https://arxiv.org/abs/2210.08402)<br>
![](https://lh5.googleusercontent.com/u4ax53sZ0oABJ2tCt4FH6fs4V6uUQ_DRirV24fX0EPpGLMZrA8OlknEohbC0L1Nctvo7hLi01R4I0a3HCfyUMnUcCm76u86ML5CyJ-5boVk_8E5BPG5Z2eeJtPDQ00IhVE-camk4)

---
### [DALL.E-3](https://openai.com/dall-e-3)
**Paper:** [Improving Image Generation with Better Captions](https://cdn.openai.com/papers/dall-e-3.pdf)<br>
**Dataset Recaptioning**<br>
![](https://github.com/rkuo2000/AI-course/raw/main/images/DALL-E3_Descriptive_Synthetic_Captions.png)

---
### [Stability.ai](https://stability.ai/)
**Code:** [Stable Diffusion](https://github.com/CompVis/stable-diffusion)
![](https://github.com/CompVis/stable-diffusion/raw/main/assets/stable-samples/txt2img/merged-0005.png)
![](https://github.com/CompVis/stable-diffusion/raw/main/assets/stable-samples/txt2img/merged-0007.png)

---
### [Imagen](https://imagen.research.google/)
**Paper:** [Photorealistic Text-to-Image Diffusion Models with Deep Language Understanding](https://arxiv.org/abs/2205.11487)<br>
**Blog:** [How Imagen Actually Works](https://www.assemblyai.com/blog/how-imagen-actually-works/)<br>
![](https://www.assemblyai.com/blog/content/images/size/w1000/2022/06/imagen_examples.png)
 
---
### SDXL
**Paper:** [SDXL: Improving Latent Diffusion Models for High-Resolution Image Synthesis](https://arxiv.org/abs/2307.01952)<br>
**Code:** [Generative Models by Stability AI](https://github.com/stability-ai/generative-models)<br>
![](https://github.com/Stability-AI/generative-models/blob/main/assets/000.jpg?raw=true)
![](https://github.com/Stability-AI/generative-models/blob/main/assets/tile.gif?raw=true)

**Huggingface:** [stable-diffusion-xl-base-1.0](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)<br>
![](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0/blob/main/pipeline.png)
SDXL consists of an ensemble of experts pipeline for latent diffusion: In a first step, the base model is used to generate (noisy) latents, which are then further processed with a refinement model (available here: https://huggingface.co/stabilityai/stable-diffusion-xl-refiner-1.0/) specialized for the final denoising steps. Note that the base model can be used as a standalone module.<br>

**Kaggle:** [https://www.kaggle.com/code/rkuo2000/sdxl-base-1-0](https://www.kaggle.com/code/rkuo2000/sdxl-base-1-0)<br>

---
### [Transfusion](https://arxiv.org/html/2408.11039v1)
**Paper:** [Transfusion: Predict the Next Token and Diffuse Images with One Multi-Modal Model](https://www.arxiv.org/abs/2408.11039)<br>
**Code:** [https://github.com/lucidrains/transfusion-pytorch](https://github.com/lucidrains/transfusion-pytorch)<br>
![](https://github.com/lucidrains/transfusion-pytorch/raw/main/transfusion.png)

---
### [FLUX1.1 pro](https://blackforestlabs.ai/announcing-flux-1-1-pro-and-the-bfl-api/)
* Superior Speed and Efficiency: Faster generation times and reduced latency, enabling more efficient workflows. FLUX1.1 [pro] is three times faster than the currently available FLUX.1 [pro]. 
* Improved Performance: FLUX1.1 [pro] has been introduced and tested under the codename “blueberry” into the Artificial Analysis image arena (https://artificialanalysis.ai/text-to-image), a popular benchmark for text-to-image models. It surpasses all other models on the leaderboard, achieving the highest overall Elo score.

---
### [SD 3.5](https://stability.ai/news/introducing-stable-diffusion-3-5)
**model:** [stabilityai/stable-diffusion-3-medium](https://huggingface.co/stabilityai/stable-diffusion-3-medium)<br>
**blog:** [ComfyUI Now Supports Stable Diffusion 3.5!](https://blog.comfy.org/sd3-5-comfyui/)<br>

---
## Deep Generative Models - Survey
**Paper**: [Personalized Image Generation with Deep Generative Models: A Decade Survey](https://arxiv.org/html/2502.13081v1)<br>
![](https://arxiv.org/html/2502.13081v1/x3.png)

---
### [OpenAI 4o Image Generation](https://openai.com/index/introducing-4o-image-generation/)
**Paper**: [An Empirical Study of GPT-4o Image Generation Capabilities](rxiv.org/abs/2504.05979)<br>

---
### [DeepMind Imagen](https://deepmind.google/models/imagen/)

---
### [Gemini NanoBanana](https://gemini.google/overview/image-generation/)

---
### Uni-COT
**Paper**: [Uni-cot: Towards Unified Chain-of-Thought Reasoning Across Text and Vision](https://arxiv.org/html/2508.05606v2)
**Code**: [https://github.com/Fr0zenCrane/UniCoT](https://github.com/Fr0zenCrane/UniCoT)<br>
<img width="50%" height="50%" src="https://github.com/Fr0zenCrane/UniCoT/raw/main/assets/qualitative_results_geo.png">
![](https://github.com/Fr0zenCrane/UniCoT/raw/main/assets/teaser.png)

---
### [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
[ComfyUI download](https://www.comfy.org/zh-cn/download)<br>

---
### Krita

#### 安裝與 ComfyUI 工作流匯入（建築景觀與室內設計應用)
<iframe width="986" height="530" src="https://www.youtube.com/embed/k8qoo1hFPic" title="Krita-AI-Diffusion 新功能教學：安裝與 ComfyUI 工作流匯入（建築景觀與室內設計應用）" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

#### FLUX.1[dev]模型在Krita完美整合
<iframe width="994" height="528" src="https://www.youtube.com/embed/Y99_C0C28UE" title="FLUX.1[dev]模型在Krita完美整合:安裝和使用教學&quot;FLUX.1[dev] in Krita: Step-by-Step Installation and Usage Tutorial&quot;" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
## Text-to-3D

### Shap-E
**Paper:** [Shap-E: Generating Conditional 3D Implicit Functions](https://arxiv.org/abs/2305.02463)<br>
**Code:** [https://github.com/openai/shap-e](https://github.com/openai/shap-e)<br>
**Kaggle:** [https://www.kaggle.com/rkuo2000/shap-e](https://www.kaggle.com/rkuo2000/shap-e)<br>

---
### [MVdiffusion](https://mvdiffusion.github.io/)
**Paper:** [MVDiffusion: Enabling Holistic Multi-view Image Generation with Correspondence-Aware Diffusion](https://arxiv.org/abs/2307.01097)<br>
**Code:** [https://github.com/Tangshitao/MVDiffusion](https://github.com/Tangshitao/MVDiffusion)<br>
![](https://github.com/Tangshitao/MVDiffusion/raw/main/assets/teaser.gif)

---
### [MVDream](https://mv-dream.github.io/)
**Paper:** [MVDream: Multi-view Diffusion for 3D Generation](https://arxiv.org/abs/2308.16512)<br>
**Code:** [https://github.com/bytedance/MVDream](https://github.com/bytedance/MVDream)<br>
**Kaggle:** [https://www.kaggle.com/rkuo2000/mvdream](https://www.kaggle.com/rkuo2000/mvdream)<br>
![](https://mv-dream.github.io/static/architecture.jpg)

---
### [3D-GPT](https://chuny1.github.io/3DGPT/3dgpt.html)
**Paper:** [3D-GPT: Procedural 3D Modeling with Large Language Models](https://arxiv.org/abs/2310.12945)<br>
![](https://chuny1.github.io/3DGPT/static/images/main.png)

---
### Advances in 3D Generation : A Survey
**Paper:** [Advances in 3D Generation: A Survey](https://arxiv.org/html/2401.17807v1)

---
### [AssetGen](https://assetgen.github.io/)
**Paper:** [Meta 3D AssetGen: Text-to-Mesh Generation with High-Quality Geometry, Texture, and PBR Materials]
(https://scontent-tpe1-1.xx.fbcdn.net/v/t39.2365-6/449707112_509645168082163_2193712134508658234_n.pdf?_nc_cat=111&ccb=1-7&_nc_sid=3c67a6&_nc_ohc=5bSbn3KaluAQ7kNvgFbjbd7&_nc_ht=scontent-tpe1-1.xx&oh=00_AYBM_JROjIFPbm8vwphinNrr4x1bUEFOeLV5iYsR6l_0rA&oe=668B3191)<br>
![](https://assetgen.github.io/static/teaser/overview.jpg)
**Paper:** [Meta 3D Gen](chrome-extension://efaidnbmnnnibpcajpcglclefindmkaj/https://scontent-tpe1-1.xx.fbcdn.net/v/t39.2365-6/449707112_509645168082163_2193712134508658234_n.pdf?_nc_cat=111&ccb=1-7&_nc_sid=3c67a6&_nc_ohc=5bSbn3KaluAQ7kNvgFbjbd7&_nc_ht=scontent-tpe1-1.xx&oh=00_AYBM_JROjIFPbm8vwphinNrr4x1bUEFOeLV5iYsR6l_0rA&oe=668B3191)

---
### AI-Render 
Stable Diffusion in Blender<br>
**Code:** [https://github.com/benrugg/AI-Render](https://github.com/benrugg/AI-Render)<br>
<iframe width="1115" height="627" src="https://www.youtube.com/embed/PXBXix2WzX4" title="AI Render - Stable Diffusion in Blender - FREE Add-on" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<iframe width="1115" height="627" src="https://www.youtube.com/embed/tmyln5bwnO8" title="AI Render Tutorial - Stable Diffusion Add-on for Blender" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<iframe width="1115" height="627" src="https://www.youtube.com/embed/zPqJUrfKuqs" title="AI Is Getting Out of Control in Blender | ControlNet" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

---
## Image-to-3D

### Zero123++
**Blog:** [Stable Zero123](https://stability.ai/news/stable-zero123-3d-generation)<br>
**Paper:** [Zero123++: a Single Image to Consistent Multi-view Diffusion Base Model](https://arxiv.org/abs/2310.15110)<br>
**Code:** [https://github.com/SUDO-AI-3D/zero123plus](https://github.com/SUDO-AI-3D/zero123plus)<br>
**Kaggle:** [https://www.kaggle.com/code/rkuo2000/zero123plus](https://www.kaggle.com/code/rkuo2000/zero123plus)<br>
**Kaggle:** [https://www.kaggle.com/code/rkuo2000/zero123-controlnet](https://www.kaggle.com/code/rkuo2000/zero123-controlnet)<br>

---
### TripoSR
**Blog:** [Introducing TripoSR: Fast 3D Object Generation from Single Images](https://stability.ai/news/triposr-3d-generation)<br>
**Paper:** [LRM: Large Reconstruction Model for Single Image to 3D](https://yiconghong.me/LRM/)<br>
**Github:** [https://github.com/VAST-AI-Research/TripoSR](https://github.com/VAST-AI-Research/TripoSR)<br>
`python run.py examples/chair.png --output-dir output/`<br>
![](https://yiconghong.me/LRM/static/images/img2nerf_model_figure.jpg)

---
### Depth Pro
**Paper:** [Depth Pro: Sharp Monocular Metric Depth in Less Than a Second](https://arxiv.org/abs/2410.02073)<br>
**Code:** [https://github.com/apple/ml-depth-pro](https://github.com/apple/ml-depth-pro)<br>
![](https://github.com/apple/ml-depth-pro/raw/main/data/depth-pro-teaser.jpg)

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*

