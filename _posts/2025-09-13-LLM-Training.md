---
layout: post # 指定文章佈局，通常是 post
title: LLM Training
date: 2025-09-13 12:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [GenAI] # 文章標籤，您可以自訂
description: LLM Training
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## Model Training

### Three Phases of Model Training
**Blog**: [解密 LLM 訓練三部曲：深入解析 SFT 與關鍵的 RLHF 技術](https://datasciocean.com/ai-concept/llm-fine-tuning-rlhf/)<br>
![](https://datasciocean.com/ai-concept/llm-fine-tuning-rlhf/llm-training-stages.png)

* 第一階段 (Self-Supervised Pre-Training)：Pre-trained LLM
* 第二階段 (Supervised Fine-Tuning)：SFT LLM
* 第三階段 (Reinforcement Learning from Human Feedback)：Reward Model 與 Final Model

---
### Pre-Train & Alignment (SFT, RLHF)
<iframe width="1264" height="711" src="https://www.youtube.com/embed/Ozos6M1JtIE?list=PLJV_el3uVTsNZEFAdQsDeOdzAaHTca2Gi" title="【生成式AI時代下的機器學習(2025)】第五講：大型語言模型訓練方法「預訓練–對齊」(Pretrain-Alignment) 的強大與極限" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Post-Training & Forgetting
<iframe width="1264" height="711" src="https://www.youtube.com/embed/Z6b5-77EfGk?list=PLJV_el3uVTsNZEFAdQsDeOdzAaHTca2Gi" title="【生成式AI時代下的機器學習(2025)】第六講：生成式人工智慧的後訓練(Post-Training)與遺忘問題" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*
