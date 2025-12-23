---
layout: post # 指定文章佈局，通常是 post
title: Model FineTuning
date: 2025-09-13 12:00:00 +0800 # 發表日期和時間 (請根據您當前的時區調整 +0800 代表 UTC+8)
categories: [Lecture] # 文章分類，您可以自訂
tags: [LLM] # 文章標籤，您可以自訂
description: Model FineTuning,  Intelligence Benchmarks
mathjax: false # 如果這篇文章不需要顯示數學公式，請設false
comments: false # 如果這篇文章需要啟用評論，請設為 true

---
## Model Training

### Three Phases of Model Training
**Blog**: [解密 LLM 訓練三部曲：深入解析 SFT 與關鍵的 RLHF 技術](https://datasciocean.com/ai-concept/llm-fine-tuning-rlhf/)<br>
* 第一階段 (Self-Supervised Pre-Training)：Pre-trained LLM
* 第二階段 (Supervised Fine-Tuning)：SFT LLM
* 第三階段 (Reinforcement Learning from Human Feedback)：Reward Model 與 Final Model
  
**Blog**: [RLHF: Reinforcement Learning from Human Feedback](https://huyenchip.com/2023/05/02/rlhf.html)
![](https://huyenchip.com/assets/pics/rlhf/1-chatgpt-training.png)

---
### Pre-Train & Alignment (SFT, RLHF)

<iframe width="1264" height="711" src="https://www.youtube.com/embed/Ozos6M1JtIE?list=PLJV_el3uVTsNZEFAdQsDeOdzAaHTca2Gi" title="【生成式AI時代下的機器學習(2025)】第五講：大型語言模型訓練方法「預訓練–對齊」(Pretrain-Alignment) 的強大與極限" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### Post-Training & Forgetting

<iframe width="1264" height="711" src="https://www.youtube.com/embed/Z6b5-77EfGk?list=PLJV_el3uVTsNZEFAdQsDeOdzAaHTca2Gi" title="【生成式AI時代下的機器學習(2025)】第六講：生成式人工智慧的後訓練(Post-Training)與遺忘問題" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---
### [Build a Large Language Model (From Scratch)](https://github.com/rasbt/LLMs-from-scratch)
**Book**: [讓 AI 好好說話！從頭打造 LLM (大型語言模型) 實戰秘笈](https://www.tenlong.com.tw/products/9789863128236?list_name=srh)<br>
![](https://cf-assets2.tenlong.com.tw/products/images/000/233/229/webp/9789863128236_%E5%A4%A9%E7%93%8F.webp?1736397148)

### [Build A Reasoning Model (From Scratch)](https://github.com/rasbt/reasoning-from-scratch)

---
## Model Fine-Tuning
**[Open-Source AI Cookbook](https://huggingface.co/learn/cookbook/en/index)** <br>

---
### SmolVLM with TRL (for ChartQA)
**Blog**: [Fine-tuning SmolVLM with TRL on a consumer GPU](https://huggingface.co/learn/cookbook/en/fine_tuning_smol_vlm_sft_trl)<br>
**Model**: [HuggingFaceTB/SmolVLM-Instruct](https://huggingface.co/HuggingFaceTB/SmolVLM-Instruct)<br>
**Dataset**: [HuggingFaceM4/ChartQA](https://huggingface.co/datasets/HuggingFaceM4/ChartQA)<br>

---
### SmolVLM with TRL (for Invoice Parser)
**Prompt**: [Fine-tuning Invoice Parser](https://chatgpt.com/share/682f9f18-7048-8010-90bb-7b27b8373a7e)<br>
**Model**: [HuggingFaceTB/SmolVLM-Instruct](https://huggingface.co/HuggingFaceTB/SmolVLM-Instruct)<br>
**Dataset**: [mychen76/invoices-and-receipts_ocr_v1](https://huggingface.co/datasets/mychen76/invoices-and-receipts_ocr_v1)<br>

---
### VLM with DPO (for Super GPT-4V)
**Blog**: [使用 TRL 對視覺語言模型進行偏好最佳化](https://huggingface.tw/blog/dpo_vlm)<br>
**Model**: [HuggingFaceM4/idefics2-8b](https://huggingface.co/HuggingFaceM4/idefics2-8b)<br>
**Dataset**: [openbmb/RLAIF-V-Dataset](https://huggingface.co/datasets/openbmb/RLAIF-V-Dataset)<br>

---
### LLM with GRPO (for GSM8K)
**Blog**: [Advanced GRPO Fine-tuning for Mathematical Reasoning with Multi-Reward Training](https://huggingface.co/learn/cookbook/en/trl_grpo_reasoning_advanced_reward)<br>
**Model**: [Qwen/Qwen2.5-3B-Instruct](https://huggingface.co/Qwen/Qwen2.5-3B-Instruct)<br>
**Dataset**: [openai/gsm8k](https://huggingface.co/datasets/openai/gsm8k)<br>

---
### VLM with GRPO (for Reasoning)
**Blog**: [Post training a VLM for reasoning with GRPO using TRL](https://huggingface.co/learn/cookbook/en/fine_tuning_vlm_grpo_trl)<br>
**Model**: [Qwen/Qwen2.5-VL-3B-Instruct](https://huggingface.co/Qwen/Qwen2.5-VL-3B-Instruct)<br>
**Dataset**: [lmms-lab/multimodal-open-r1-8k-verified](https://huggingface.co/datasets/lmms-lab/multimodal-open-r1-8k-verified)<br>
![](https://github.com/rkuo2000/AI-course/blob/main/assets/images/PPO_vs_GRPO.jpg?raw=true)

---
## Intelligence Benchmarks

### [OpenAI Evals](https://evals.openai.com/)

---
### SWE-Bench
**Paper**: [SWE-bench: Can Language Models Resolve Real-World GitHub Issues?](https://arxiv.org/abs/2310.06770)<br>
**Code**: [https://github.com/SWE-bench/SWE-bench](https://github.com/SWE-bench/SWE-bench)<br>

---
### MLE-Bench
**Paper**: [MLE-bench: Evaluating Machine Learning Agents on Machine Learning Engineering](https://arxiv.org/abs/2410.07095)<br>
**Code**: [https://github.com/openai/mle-bench](https://github.com/openai/mle-bench)<br>

---
### SWE-Lancer
**Paper**: [SWE-Lancer: Can Frontier LLMs Earn $1 Million from Real-World Freelance Software Engineering?](https://arxiv.org/abs/2502.12115)<br>

### PaperBench
**Paper**: [PaperBench: Evaluating AI's Ability to Replicate AI Research](https://arxiv.org/abs/2504.01848)<br>
**Code**: [https://github.com/openai/frontier-evals](https://github.com/openai/frontier-evals)<br>

---
### SWE-Bench Pro
**Paper**: [SWE-Bench Pro: Can AI Agents Solve Long-Horizon Software Engineering Tasks?](https://arxiv.org/abs/2509.16941)<br>
**Code**: [https://github.com/scaleapi/SWE-bench_Pro-os](https://github.com/scaleapi/SWE-bench_Pro-os)<br>

---
### GPDval
**Paper**: [GDPval: Evaluating AI Model Performance on Real-World Economically Valuable Tasks](https://arxiv.org/abs/2510.04374)<br>
![](https://arxiv.org/html/2510.04374v1/exampletasksscreenshot.png)
**Dataset**: [https://huggingface.co/datasets/openai/gdpval](https://huggingface.co/datasets/openai/gdpval)<br>
* 220 real-world knowledge tasks across 44 occupations.
* Each task consists of a text prompt and a set of supporting reference files.

---
### ToolOrchestra
**Paper**: [ToolOrchestra: Elevating Intelligence via Efficient Model and Tool Orchestration](https://arxiv.org/abs/2511.21689)<br>
**Code**: [https://github.com/NVlabs/ToolOrchestra](https://github.com/NVlabs/ToolOrchestra)<br>
![](https://raw.githubusercontent.com/NVlabs/ToolOrchestra/main/assets/method.png)

---
### RLVR
**Paper**: [Reinforcement Learning with Verifiable Rewards Implicitly Incentivizes Correct Reasoning in Base LLMs](https://arxiv.org/html/2506.14245v2)<br>

<br>
<br>

*This site was last updated {{ site.time | date: "%B %d, %Y" }}.*
