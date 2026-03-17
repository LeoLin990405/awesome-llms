<div align="center">

# Awesome LLMs / 大语言模型精选列表

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![GitHub stars](https://img.shields.io/github/stars/LeoLin990405/awesome-llms?style=social)](https://github.com/LeoLin990405/awesome-llms/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/LeoLin990405/awesome-llms)](https://github.com/LeoLin990405/awesome-llms/issues)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/LeoLin990405/awesome-llms/pulls)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

A curated bilingual (EN/中文) list of Large Language Models, tools, benchmarks, and resources.

精选大语言模型、工具、基准测试与学习资源的中英文对照列表。

</div>

**Last updated / 最后更新: 2026-03-16**

---

## Table of Contents / 目录

- [Flagship Proprietary Models / 旗舰闭源模型](#flagship-proprietary-models--旗舰闭源模型)
- [Open-Source General Models / 开源通用模型](#open-source-general-models--开源通用模型)
- [Chinese LLMs / 中国大模型](#chinese-llms--中国大模型)
- [Reasoning Models / 推理模型](#reasoning-models--推理模型)
- [Code Generation Models / 代码生成模型](#code-generation-models--代码生成模型)
- [Multimodal & Vision-Language Models / 多模态与视觉语言模型](#multimodal--vision-language-models--多模态与视觉语言模型)
- [Small Language Models & Edge / 小语言模型与端侧部署](#small-language-models--edge--小语言模型与端侧部署)
- [Embedding Models / 嵌入模型](#embedding-models--嵌入模型)
- [Domain-Specific Models / 领域专用模型](#domain-specific-models--领域专用模型)
- [Model Serving & Inference / 模型服务与推理](#model-serving--inference--模型服务与推理)
- [Fine-Tuning & Training / 微调与训练](#fine-tuning--training--微调与训练)
- [Evaluation & Benchmarks / 评测与基准测试](#evaluation--benchmarks--评测与基准测试)
- [API Providers & Aggregators / API 提供商与聚合平台](#api-providers--aggregators--api-提供商与聚合平台)
- [Learning Resources / 学习资源](#learning-resources--学习资源)
- [Contributing / 贡献指南](#contributing--贡献指南)

---

## Flagship Proprietary Models / 旗舰闭源模型

> Closed-source models accessible via API from major providers / 主要厂商提供的闭源 API 模型

### OpenAI

| Model / 模型 | Parameters / 参数 | Context / 上下文 | Description / 描述 | Pricing (per 1M tokens) / 价格 |
|---|---|---|---|---|
| [GPT-5](https://openai.com/) | Undisclosed / 未公开 | 256K | Most capable all-purpose model, top benchmark scores / 最强通用模型，基准测试榜首 | $5 / $15 |
| [GPT-4.1](https://openai.com/) | Undisclosed / 未公开 | 1M | Optimized for coding & instruction following / 代码与指令遵循优化 | $2 / $8 |
| [GPT-4o](https://openai.com/) | Undisclosed / 未公开 | 128K | Multimodal (text+image+audio), fast / 多模态(文本+图像+音频)，快速 | $2.50 / $10 |
| [GPT-5-mini](https://openai.com/) | Undisclosed / 未公开 | 128K | Budget-friendly, fast responses / 经济实惠，响应快速 | $0.25 / $2 |

### Anthropic

| Model / 模型 | Parameters / 参数 | Context / 上下文 | Description / 描述 | Pricing (per 1M tokens) / 价格 |
|---|---|---|---|---|
| [Claude Opus 4.6](https://anthropic.com/) | Undisclosed / 未公开 | 200K | Deepest reasoning, extended thinking mode / 最深度推理，扩展思考模式 | $15 / $75 |
| [Claude Sonnet 4.6](https://anthropic.com/) | Undisclosed / 未公开 | 200K | Best balance of speed and intelligence / 速度与智能最佳平衡 | $3 / $15 |
| [Claude Haiku 4.5](https://anthropic.com/) | Undisclosed / 未公开 | 200K | Fastest, most affordable Claude / 最快最经济的 Claude | $1 / $5 |

### Google DeepMind

| Model / 模型 | Parameters / 参数 | Context / 上下文 | Description / 描述 | Pricing (per 1M tokens) / 价格 |
|---|---|---|---|---|
| [Gemini 3 Pro](https://deepmind.google/) | Undisclosed / 未公开 | 2M | Top-tier with Deep Think reasoning / 旗舰级深度思考推理 | $3.50 / $10.50 |
| [Gemini 2.5 Flash](https://deepmind.google/) | Undisclosed / 未公开 | 1M | Fast, cost-efficient, thinking mode / 快速高效，思考模式 | $0.15 / $0.60 |
| [Gemini 2.5 Pro](https://deepmind.google/) | Undisclosed / 未公开 | 1M | Strong coding & reasoning / 强编程与推理 | $1.25 / $5 |

### xAI

| Model / 模型 | Parameters / 参数 | Context / 上下文 | Description / 描述 | Pricing (per 1M tokens) / 价格 |
|---|---|---|---|---|
| [Grok-3](https://x.ai/) | Undisclosed / 未公开 | 128K | Real-time data access, strong reasoning / 实时数据访问，强推理能力 | $3 / $15 |
| [Grok-3 Mini](https://x.ai/) | Undisclosed / 未公开 | 128K | Lightweight, fast thinking mode / 轻量快速，思考模式 | $0.30 / $0.50 |

### Amazon

| Model / 模型 | Parameters / 参数 | Context / 上下文 | Description / 描述 | Pricing (per 1M tokens) / 价格 |
|---|---|---|---|---|
| [Nova Pro](https://aws.amazon.com/bedrock/) | Undisclosed / 未公开 | 300K | Multimodal, strong on Bedrock / 多模态，Bedrock 平台强力模型 | $0.80 / $3.20 |
| [Nova Lite](https://aws.amazon.com/bedrock/) | Undisclosed / 未公开 | 300K | Budget multimodal / 经济多模态 | $0.06 / $0.24 |

---

## Open-Source General Models / 开源通用模型

> Open-weight models available for download and self-hosting / 可下载与自部署的开源权重模型

### Meta — Llama Series / Meta — Llama 系列

| Model / 模型 | Parameters / 参数 | Architecture / 架构 | Description / 描述 | License / 许可 |
|---|---|---|---|---|
| [Llama 4 Maverick](https://github.com/meta-llama/llama4) | 400B (17B active) | MoE | Flagship MoE, multimodal (text+image) / 旗舰 MoE，多模态 | Llama 4 |
| [Llama 4 Scout](https://github.com/meta-llama/llama4) | 109B (17B active) | MoE | 10M context window, efficient / 千万级上下文，高效 | Llama 4 |
| [Llama 3.3](https://github.com/meta-llama/llama3) | 70B | Dense | Versatile, strong instruction following / 通用性强，指令遵循好 | Llama 3.3 |
| [Llama 3.2](https://github.com/meta-llama/llama3) | 1B / 3B / 11B / 90B | Dense | Edge-friendly sizes, vision variants / 端侧友好，视觉变体 | Llama 3.2 |

### Alibaba — Qwen Series / 阿里巴巴 — 通义千问系列

| Model / 模型 | Parameters / 参数 | Architecture / 架构 | Description / 描述 | License / 许可 |
|---|---|---|---|---|
| [Qwen3.5-397B-A17B](https://github.com/QwenLM/Qwen3) | 397B (17B active) | MoE | Latest flagship, multimodal + ultra-long context / 最新旗舰，多模态+超长上下文 | Apache 2.0 |
| [Qwen3-235B-A22B](https://github.com/QwenLM/Qwen3) | 235B (22B active) | MoE | Hybrid thinking, beats GPT-4o on benchmarks / 混合思考，基准超越 GPT-4o | Apache 2.0 |
| [Qwen3-32B](https://github.com/QwenLM/Qwen3) | 32B | Dense | Best dense model at this scale / 该规模最佳稠密模型 | Apache 2.0 |
| [Qwen3-8B](https://github.com/QwenLM/Qwen3) | 8B | Dense | Great for local deployment / 本地部署优选 | Apache 2.0 |

### Mistral AI

| Model / 模型 | Parameters / 参数 | Architecture / 架构 | Description / 描述 | License / 许可 |
|---|---|---|---|---|
| [Mistral Large 3](https://github.com/mistralai/) | 675B (41B active) | MoE | 92% of GPT-5.2 at 15% cost / 92% GPT-5.2 性能，15% 成本 | Apache 2.0 |
| [Mistral 3 14B](https://github.com/mistralai/) | 14B | Dense | Top small dense model / 顶级小型稠密模型 | Apache 2.0 |
| [Mistral 3 8B](https://github.com/mistralai/) | 8B | Dense | Fast, efficient for edge / 快速高效，适合边缘部署 | Apache 2.0 |
| [Mistral 3 3B](https://github.com/mistralai/) | 3B | Dense | Smallest Mistral 3, mobile-ready / 最小 Mistral 3，移动端可用 | Apache 2.0 |
| [Mistral Nemo](https://github.com/mistralai/) | 12B | Dense | Strong general purpose / 通用性强 | Apache 2.0 |

### OpenAI Open-Weight / OpenAI 开源权重

| Model / 模型 | Parameters / 参数 | Architecture / 架构 | Description / 描述 | License / 许可 |
|---|---|---|---|---|
| [GPT-oss-120B](https://openai.com/) | 120B | Dense | First open-weight from OpenAI / OpenAI 首个开源权重模型 | Apache 2.0 |
| [GPT-oss-20B](https://openai.com/) | 20B | Dense | Lightweight open-weight variant / 轻量开源变体 | Apache 2.0 |

### Other Notable Models / 其他重要模型

| Model / 模型 | Organization / 机构 | Parameters / 参数 | Description / 描述 | License / 许可 |
|---|---|---|---|---|
| [Falcon-180B](https://huggingface.co/tiiuae/falcon-180B) | TII (UAE) | 180B | Large-scale open model / 大规模开放模型 | Falcon License |
| [Yi-Large](https://github.com/01-ai/Yi) | 01.AI (李开复) | 200B+ | Bilingual EN/ZH powerhouse / 中英双语强模型 | Yi License |
| [Command R+](https://cohere.com/) | Cohere | 104B | Enterprise RAG optimized / 企业 RAG 优化 | CC-BY-NC |
| [DBRX](https://github.com/databricks/dbrx) | Databricks | 132B (36B active) | MoE, enterprise-grade / MoE，企业级 | Databricks Open |
| [Jamba 1.5](https://www.ai21.com/) | AI21 Labs | 398B (94B active) | SSM+Transformer hybrid, 256K ctx / SSM+Transformer 混合，256K 上下文 | Apache 2.0 |
| [OLMo 2](https://github.com/allenai/OLMo) | Allen AI | 7B / 13B | Fully open (weights+data+code) / 完全开放(权重+数据+代码) | Apache 2.0 |

---

## Chinese LLMs / 中国大模型

> Models developed by Chinese companies and research institutions / 中国公司与研究机构开发的模型

| Model / 模型 | Organization / 机构 | Parameters / 参数 | Description / 描述 | Stars |
|---|---|---|---|---|
| [DeepSeek-V3](https://github.com/deepseek-ai/DeepSeek-V3) | DeepSeek (深度求索) | 671B (37B active) | Top open-source MoE, extremely cost-effective / 顶级开源 MoE，极致性价比 | ![Stars](https://img.shields.io/github/stars/deepseek-ai/DeepSeek-V3) |
| [Qwen3](https://github.com/QwenLM/Qwen3) | Alibaba (阿里巴巴) | 0.6B–397B | ↗ [Details / 详情](#alibaba--qwen-series--阿里巴巴--通义千问系列) | ![Stars](https://img.shields.io/github/stars/QwenLM/Qwen3) |
| [Kimi K2](https://github.com/MoonshotAI/Kimi-K2) | Moonshot AI (月之暗面) | 1T+ (32B active) | Best non-Western model by benchmarks / 基准测试最强非西方模型 | ![Stars](https://img.shields.io/github/stars/MoonshotAI/Kimi-K2) |
| [GLM-4](https://github.com/THUDM/GLM-4) | Zhipu AI (智谱AI) | 9B / 130B | 1M context, 26 languages, strong multi-turn / 百万上下文，26种语言，多轮对话强 | ![Stars](https://img.shields.io/github/stars/THUDM/GLM-4) |
| [Doubao 1.5 Pro](https://www.volcengine.com/) | ByteDance (字节跳动) | MoE | Sparse MoE, powers Doubao app / 稀疏 MoE，驱动豆包应用 | — |
| [Ernie 4.5](https://github.com/PaddlePaddle/ERNIE) | Baidu (百度) | Undisclosed / 未公开 | Enterprise-focused, integrated with Baidu Cloud / 企业级，百度云集成 | ![Stars](https://img.shields.io/github/stars/PaddlePaddle/ERNIE) |
| [Hunyuan](https://github.com/Tencent/HunyuanLLM) | Tencent (腾讯) | MoE | Multimodal, WeChat ecosystem / 多模态，微信生态 | ![Stars](https://img.shields.io/github/stars/Tencent/HunyuanLLM) |
| [InternLM3](https://github.com/InternLM/InternLM) | Shanghai AI Lab (上海AI实验室) | 8B / 20B | Research-focused, strong tool use / 研究导向，工具使用强 | ![Stars](https://img.shields.io/github/stars/InternLM/InternLM) |
| [Yi-Large](https://github.com/01-ai/Yi) | 01.AI (零一万物) | 200B+ | Bilingual EN/ZH, by Kai-Fu Lee / 中英双语，李开复创立 | ![Stars](https://img.shields.io/github/stars/01-ai/Yi) |
| [MiniMax-01](https://github.com/MiniMax-AI) | MiniMax | 456B (45.9B active) | Lightning attention, 1M context / 闪电注意力，百万上下文 | — |
| [Skywork](https://github.com/SkyworkAI/Skywork) | Kunlun Tech (昆仑万维) | 13B | Open-source, strong on Chinese benchmarks / 开源，中文基准表现优异 | ![Stars](https://img.shields.io/github/stars/SkyworkAI/Skywork) |
| [Baichuan 4](https://github.com/baichuan-inc/Baichuan2) | Baichuan (百川智能) | Various | Enterprise AI assistant platform / 企业AI助手平台 | ![Stars](https://img.shields.io/github/stars/baichuan-inc/Baichuan2) |
| [Pangu](https://www.huaweicloud.com/) | Huawei (华为) | Various | Industry-specific models on Huawei Cloud / 华为云行业专用模型 | — |
| [Spark](https://xinghuo.xfyun.cn/) | iFlytek (科大讯飞) | Various | Strong in speech + NLP / 语音+NLP 领域强 | — |
| [Abab](https://www.minimaxi.com/) | MiniMax | Various | Powers Talkie & Hailuo AI / 驱动 Talkie 与海螺AI | — |

---

## Reasoning Models / 推理模型

> Models with explicit chain-of-thought reasoning capabilities / 具有显式思维链推理能力的模型

| Model / 模型 | Organization / 机构 | Type / 类型 | Description / 描述 | Open Source / 开源 |
|---|---|---|---|---|
| [o3](https://openai.com/) | OpenAI | Proprietary / 闭源 | Strongest reasoning model, excels at math & science / 最强推理模型，数学与科学卓越 | No / 否 |
| [o4-mini](https://openai.com/) | OpenAI | Proprietary / 闭源 | Fast reasoning, cost-effective / 快速推理，性价比高 | No / 否 |
| [DeepSeek-R1](https://github.com/deepseek-ai/DeepSeek-R1) | DeepSeek | Open / 开源 | Matches o1 on math/code, RL-trained CoT / 数学/代码媲美 o1，RL 训练思维链 | ![Stars](https://img.shields.io/github/stars/deepseek-ai/DeepSeek-R1) |
| [DeepSeek-R1-Distill](https://github.com/deepseek-ai/DeepSeek-R1) | DeepSeek | Open / 开源 | Distilled R1 in smaller sizes (1.5B–70B) / R1 蒸馏版(1.5B–70B) | ![Stars](https://img.shields.io/github/stars/deepseek-ai/DeepSeek-R1) |
| [QwQ-32B](https://github.com/QwenLM/QwQ) | Alibaba | Open / 开源 | 32B reasoning model, strong on AIME / 32B 推理模型，AIME 表现优异 | ![Stars](https://img.shields.io/github/stars/QwenLM/QwQ) |
| [Qwen3 (Thinking Mode)](https://github.com/QwenLM/Qwen3) | Alibaba | Open / 开源 | Hybrid thinking/non-thinking, switchable / 混合思考/非思考，可切换 | ![Stars](https://img.shields.io/github/stars/QwenLM/Qwen3) |
| [Gemini Deep Think](https://deepmind.google/) | Google | Proprietary / 闭源 | Extended reasoning within Gemini 3 Pro / Gemini 3 Pro 扩展推理 | No / 否 |
| [Claude Extended Thinking](https://anthropic.com/) | Anthropic | Proprietary / 闭源 | Up to 64K output tokens in thinking mode / 思考模式最多 64K 输出 | No / 否 |
| [Kimi Thinking](https://www.moonshot.cn/) | Moonshot AI | Proprietary / 闭源 | Step-by-step reasoning chain / 逐步推理链 | No / 否 |
| [Grok-3 Think](https://x.ai/) | xAI | Proprietary / 闭源 | Reasoning variant of Grok-3 / Grok-3 推理变体 | No / 否 |
| [Marco-o1](https://github.com/AIDC-AI/Marco-o1) | Alibaba DAMO | Open / 开源 | Open-source o1-style reasoning / 开源 o1 风格推理 | ![Stars](https://img.shields.io/github/stars/AIDC-AI/Marco-o1) |
| [Sky-T1](https://github.com/NovaSky-AI/Sky-T1-32B-Preview) | NovaSky | Open / 开源 | 32B reasoning, community-driven / 32B 推理，社区驱动 | ![Stars](https://img.shields.io/github/stars/NovaSky-AI/Sky-T1-32B-Preview) |

---

## Code Generation Models / 代码生成模型

> Models specialized for coding, debugging, and software engineering / 专注编程、调试与软件工程的模型

| Model / 模型 | Organization / 机构 | Parameters / 参数 | Description / 描述 | Stars |
|---|---|---|---|---|
| [Qwen3-Coder](https://github.com/QwenLM/Qwen3-Coder) | Alibaba | 480B (35B active) | Ultra-sparse MoE, best open coding model / 超稀疏 MoE，最佳开源编码模型 | ![Stars](https://img.shields.io/github/stars/QwenLM/Qwen3-Coder) |
| [DeepSeek-Coder-V2](https://github.com/deepseek-ai/DeepSeek-Coder-V2) | DeepSeek | 236B (21B active) | MoE coder, strong algorithmic ability / MoE 编码模型，算法能力强 | ![Stars](https://img.shields.io/github/stars/deepseek-ai/DeepSeek-Coder-V2) |
| [Kimi-Dev-72B](https://github.com/MoonshotAI/Kimi-Dev-72B) | Moonshot AI | 72B | Top SWE-bench scores, agentic coding / SWE-bench 顶级分数，智能体编码 | ![Stars](https://img.shields.io/github/stars/MoonshotAI/Kimi-Dev-72B) |
| [StarCoder2](https://github.com/bigcode-project/starcoder2) | BigCode | 3B / 7B / 15B | 17 languages, community-built / 17种语言，社区共建 | ![Stars](https://img.shields.io/github/stars/bigcode-project/starcoder2) |
| [CodeLlama](https://github.com/meta-llama/codellama) | Meta | 7B / 13B / 34B / 70B | Based on Llama 2, code-specialized / 基于 Llama 2，代码专用 | ![Stars](https://img.shields.io/github/stars/meta-llama/codellama) |
| [Codestral](https://mistral.ai/) | Mistral | 22B | Optimized for code, 80+ languages / 代码优化，80+ 语言 | — |
| [CodeGeeX4](https://github.com/THUDM/CodeGeeX4) | Zhipu AI | 9B | Multilingual, IDE plugins / 多语言，IDE 插件 | ![Stars](https://img.shields.io/github/stars/THUDM/CodeGeeX4) |
| [OpenCoder](https://github.com/infly-ai/OpenCoder) | InfLy | 1.5B / 8B | Fully open (code+data+recipes) / 完全开放(代码+数据+训练方案) | ![Stars](https://img.shields.io/github/stars/infly-ai/OpenCoder) |
| [Granite Code](https://github.com/ibm-granite/granite-code-models) | IBM | 3B–34B | Enterprise code, 116 languages / 企业级代码，116种语言 | ![Stars](https://img.shields.io/github/stars/ibm-granite/granite-code-models) |
| [WizardCoder](https://github.com/nlpxucan/WizardLM) | WizardLM Team | 15B / 34B | Evol-Instruct for code / 代码进化指令调优 | ![Stars](https://img.shields.io/github/stars/nlpxucan/WizardLM) |
| [Devstral](https://mistral.ai/) | Mistral | 24B | Agentic coding, SWE-bench optimized / 智能体编码，SWE-bench 优化 | — |

---

## Multimodal & Vision-Language Models / 多模态与视觉语言模型

> Models that process text, images, audio, and/or video / 处理文本、图像、音频和/或视频的模型

### Proprietary Multimodal / 闭源多模态

| Model / 模型 | Modalities / 模态 | Description / 描述 |
|---|---|---|
| [GPT-4o](https://openai.com/) | Text + Image + Audio / 文本+图像+音频 | Native multimodal, fast / 原生多模态，快速 |
| [Gemini 3 Pro](https://deepmind.google/) | Text + Image + Audio + Video / 全模态 | Best video understanding / 最强视频理解 |
| [Claude Opus 4.6](https://anthropic.com/) | Text + Image / 文本+图像 | Deep image analysis / 深度图像分析 |
| [Grok-3 Vision](https://x.ai/) | Text + Image / 文本+图像 | Real-time image understanding / 实时图像理解 |

### Open-Source Multimodal / 开源多模态

| Model / 模型 | Parameters / 参数 | Modalities / 模态 | Description / 描述 | Stars |
|---|---|---|---|---|
| [Qwen2.5-VL](https://github.com/QwenLM/Qwen2.5-VL) | 3B / 7B / 72B | Text + Image + Video | Top DocVQA scores, beats GPT-4o on OCR / 文档VQA 最佳，OCR 超越 GPT-4o | ![Stars](https://img.shields.io/github/stars/QwenLM/Qwen2.5-VL) |
| [InternVL3](https://github.com/OpenGVLab/InternVL) | 1B–78B | Text + Image + Video | Versatile VLM, strong benchmarks / 通用 VLM，基准表现强 | ![Stars](https://img.shields.io/github/stars/OpenGVLab/InternVL) |
| [Llama 4 Maverick](https://github.com/meta-llama/llama4) | 400B (17B active) | Text + Image | ↗ [Details / 详情](#meta--llama-series--meta--llama-系列) | ![Stars](https://img.shields.io/github/stars/meta-llama/llama4) |
| [LLaVA-OneVision](https://github.com/LLaVA-VL/LLaVA-NeXT) | 7B / 72B | Text + Image + Video | Leading open VLM family / 领先开源 VLM 系列 | ![Stars](https://img.shields.io/github/stars/LLaVA-VL/LLaVA-NeXT) |
| [Pixtral Large](https://github.com/mistralai/) | 124B | Text + Image | Mistral's vision model / Mistral 视觉模型 | — |
| [Gemma 3](https://github.com/google-deepmind/gemma) | 4B / 12B / 27B | Text + Image | Native vision, 128K context / 原生视觉，128K 上下文 | ![Stars](https://img.shields.io/github/stars/google-deepmind/gemma) |
| [CogVLM2](https://github.com/THUDM/CogVLM2) | 19B | Text + Image + Video | Strong visual grounding / 强视觉定位 | ![Stars](https://img.shields.io/github/stars/THUDM/CogVLM2) |
| [Idefics3](https://huggingface.co/HuggingFaceM4/Idefics3-8B-Llama3) | 8B | Text + Image | Hugging Face's open VLM / Hugging Face 开源 VLM | — |
| [DeepSeek-VL2](https://github.com/deepseek-ai/DeepSeek-VL2) | 4.5B / 16B / 27B | Text + Image | MoE vision-language / MoE 视觉语言 | ![Stars](https://img.shields.io/github/stars/deepseek-ai/DeepSeek-VL2) |
| [MiniCPM-V](https://github.com/OpenBMB/MiniCPM-V) | 3B / 8B | Text + Image | Phone-deployable, strong OCR / 手机端可部署，OCR 强 | ![Stars](https://img.shields.io/github/stars/OpenBMB/MiniCPM-V) |

### Audio & Speech Models / 音频与语音模型

| Model / 模型 | Organization / 机构 | Description / 描述 | Stars |
|---|---|---|---|
| [Whisper](https://github.com/openai/whisper) | OpenAI | Best open ASR, 99 languages / 最佳开源语音识别，99种语言 | ![Stars](https://img.shields.io/github/stars/openai/whisper) |
| [Qwen2-Audio](https://github.com/QwenLM/Qwen2-Audio) | Alibaba | Audio understanding & generation / 音频理解与生成 | ![Stars](https://img.shields.io/github/stars/QwenLM/Qwen2-Audio) |
| [SALMONN](https://github.com/bytedance/SALMONN) | ByteDance | Speech + audio + music LLM / 语音+音频+音乐 LLM | ![Stars](https://img.shields.io/github/stars/bytedance/SALMONN) |
| [Moshi](https://github.com/kyutai-labs/moshi) | Kyutai | Real-time speech dialogue / 实时语音对话 | ![Stars](https://img.shields.io/github/stars/kyutai-labs/moshi) |

---

## Small Language Models & Edge / 小语言模型与端侧部署

> Compact models optimized for edge devices, mobile, and on-device inference / 为边缘设备、移动端和端侧推理优化的紧凑模型

| Model / 模型 | Organization / 机构 | Parameters / 参数 | Description / 描述 | Stars |
|---|---|---|---|---|
| [Phi-4](https://github.com/microsoft/phi-4) | Microsoft | 14B | Beats GPT-4o on MATH, curated data training / MATH 超越 GPT-4o，精选数据训练 | ![Stars](https://img.shields.io/github/stars/microsoft/phi-4) |
| [Phi-4-mini](https://github.com/microsoft/phi-4) | Microsoft | 3.8B | Phone-ready, strong reasoning for size / 手机端可用，同规模推理强 | ![Stars](https://img.shields.io/github/stars/microsoft/phi-4) |
| [Gemma 3](https://github.com/google-deepmind/gemma) | Google | 1B / 4B / 12B / 27B | ↗ [Details / 详情](#open-source-multimodal--开源多模态) | ![Stars](https://img.shields.io/github/stars/google-deepmind/gemma) |
| [Llama 3.2](https://github.com/meta-llama/llama3) | Meta | 1B / 3B | 650MB RAM with 4-bit quant, 20-30 tok/s on iPhone / 4位量化650MB内存，iPhone 20-30 tok/s | ![Stars](https://img.shields.io/github/stars/meta-llama/llama3) |
| [Qwen3-0.6B / 1.7B / 4B](https://github.com/QwenLM/Qwen3) | Alibaba | 0.6B–4B | Smallest Qwen, edge-ready / 最小 Qwen，端侧就绪 | ![Stars](https://img.shields.io/github/stars/QwenLM/Qwen3) |
| [Mistral 3 3B](https://mistral.ai/) | Mistral | 3B | Smallest Mistral, mobile-ready / 最小 Mistral，移动端可用 | — |
| [SmolLM2](https://github.com/huggingface/smollm) | Hugging Face | 135M / 360M / 1.7B | Ultra-small, on-device / 超小型，端上运行 | ![Stars](https://img.shields.io/github/stars/huggingface/smollm) |
| [TinyLlama](https://github.com/jzhang38/TinyLlama) | Community | 1.1B | 3T tokens trained, tiny but capable / 3T token 训练，小巧但能干 | ![Stars](https://img.shields.io/github/stars/jzhang38/TinyLlama) |
| [MiniCPM](https://github.com/OpenBMB/MiniCPM) | OpenBMB / Tsinghua | 1.2B / 2.4B | Chinese SLM, phone deployment / 中文小模型，手机端部署 | ![Stars](https://img.shields.io/github/stars/OpenBMB/MiniCPM) |
| [Stable LM 2](https://github.com/Stability-AI/StableLM) | Stability AI | 1.6B / 12B | Compact, efficient / 紧凑高效 | ![Stars](https://img.shields.io/github/stars/Stability-AI/StableLM) |

---

## Embedding Models / 嵌入模型

> Models for converting text/images to vector representations for search, RAG, etc. / 将文本/图像转换为向量表示的模型，用于搜索、RAG 等

| Model / 模型 | Organization / 机构 | Dimensions / 维度 | Description / 描述 | Type / 类型 |
|---|---|---|---|---|
| [text-embedding-3-large](https://openai.com/) | OpenAI | 3072 | Best overall API embedding / 最佳综合 API 嵌入 | API |
| [text-embedding-3-small](https://openai.com/) | OpenAI | 1536 | Cost-effective, fast / 经济实惠，快速 | API |
| [Voyage-3-large](https://www.voyageai.com/) | Voyage AI | 2048 | Top MTEB retrieval scores / MTEB 检索最高分 | API |
| [Cohere Embed v4](https://cohere.com/) | Cohere | 1024 | Text + image in same vector space / 文本+图像同一向量空间 | API |
| [BGE-M3](https://github.com/FlagOpen/FlagEmbedding) | BAAI (北京智源) | 1024 | Multi-lingual, multi-granularity / 多语言，多粒度 | Open / 开源 |
| [BGE-large-en-v1.5](https://github.com/FlagOpen/FlagEmbedding) | BAAI (北京智源) | 1024 | Strong English embedding / 强英文嵌入 | Open / 开源 |
| [GTE-Qwen2](https://github.com/ContextualAI/gritlm) | Alibaba | 768–4096 | Scaling embedding with Qwen backbone / Qwen 骨干扩展嵌入 | Open / 开源 |
| [E5-Mistral-7B](https://huggingface.co/intfloat/e5-mistral-7b-instruct) | Microsoft | 4096 | LLM-based embedding / 基于 LLM 的嵌入 | Open / 开源 |
| [Nomic Embed](https://github.com/nomic-ai/nomic-embed-text-v1.5) | Nomic AI | 768 | Fully open, strong for size / 完全开源，同规模强 | Open / 开源 |
| [Jina Embeddings v3](https://jina.ai/) | Jina AI | 1024 | Task-specific LoRA adapters / 任务专用 LoRA 适配器 | API + Open |
| [Gemini Embedding](https://deepmind.google/) | Google | 3072 | Google's latest embedding model / 谷歌最新嵌入模型 | API |

---

## Domain-Specific Models / 领域专用模型

> Models fine-tuned or designed for specific industries and tasks / 为特定行业和任务微调或设计的模型

### Medical & Healthcare / 医疗与健康

| Model / 模型 | Description / 描述 | Stars |
|---|---|---|
| [Med-PaLM 2](https://sites.research.google/med-palm/) | Google's medical QA model, expert-level / 谷歌医学问答模型，专家水平 | — |
| [BioMistral](https://github.com/BioMistral/BioMistral) | Open medical LLM based on Mistral / 基于 Mistral 的开源医学 LLM | ![Stars](https://img.shields.io/github/stars/BioMistral/BioMistral) |
| [HuatuoGPT](https://github.com/FreedomIntelligence/HuatuoGPT) | Chinese medical LLM (华佗GPT) / 中文医学大模型 | ![Stars](https://img.shields.io/github/stars/FreedomIntelligence/HuatuoGPT) |
| [XingShi (行实)](https://www.fangzhou.ai/) | Chinese healthcare chronic disease management / 中国医疗慢病管理 | — |

### Legal / 法律

| Model / 模型 | Description / 描述 | Stars |
|---|---|---|
| [ChatLaw](https://github.com/PKU-YuanGroup/ChatLaw) | Chinese legal LLM (北大) / 中文法律大模型(北大) | ![Stars](https://img.shields.io/github/stars/PKU-YuanGroup/ChatLaw) |
| [SaulLM](https://github.com/Equall-AI/saul-7b) | Legal domain LLM / 法律领域大模型 | ![Stars](https://img.shields.io/github/stars/Equall-AI/saul-7b) |

### Finance / 金融

| Model / 模型 | Description / 描述 | Stars |
|---|---|---|
| [FinGPT](https://github.com/AI4Finance-Foundation/FinGPT) | Open-source financial LLM / 开源金融大模型 | ![Stars](https://img.shields.io/github/stars/AI4Finance-Foundation/FinGPT) |
| [BloombergGPT](https://arxiv.org/abs/2303.17564) | 50B financial model / 500亿参数金融模型 | — |
| [XUANYUAN](https://github.com/Duxiaoman-DI/XuanYuan) | Chinese finance LLM (度小满轩辕) / 中文金融大模型 | ![Stars](https://img.shields.io/github/stars/Duxiaoman-DI/XuanYuan) |

### Science & Math / 科学与数学

| Model / 模型 | Description / 描述 | Stars |
|---|---|---|
| [DeepSeek-Prover-V2](https://github.com/deepseek-ai/DeepSeek-Prover-V2) | Formal theorem proving in Lean 4 / Lean 4 形式化定理证明 | ![Stars](https://img.shields.io/github/stars/deepseek-ai/DeepSeek-Prover-V2) |
| [Llemma](https://github.com/EleutherAI/math-lm) | Math-specialized open model / 数学专用开源模型 | ![Stars](https://img.shields.io/github/stars/EleutherAI/math-lm) |
| [Galactica](https://github.com/paperswithcode/galai) | Scientific knowledge LLM / 科学知识大模型 | ![Stars](https://img.shields.io/github/stars/paperswithcode/galai) |
| [SciGLM](https://github.com/THUDM/SciGLM) | Scientific reasoning LLM (清华) / 科学推理大模型 | ![Stars](https://img.shields.io/github/stars/THUDM/SciGLM) |

---

## Model Serving & Inference / 模型服务与推理

> Tools for deploying and running LLMs efficiently / 高效部署和运行大模型的工具

| Tool / 工具 | Description / 描述 | Stars |
|---|---|---|
| [vLLM](https://github.com/vllm-project/vllm) | High-throughput LLM serving with PagedAttention / 高吞吐量 PagedAttention 推理服务 | ![Stars](https://img.shields.io/github/stars/vllm-project/vllm) |
| [Ollama](https://github.com/ollama/ollama) | Run LLMs locally with one command / 一条命令本地运行大模型 | ![Stars](https://img.shields.io/github/stars/ollama/ollama) |
| [llama.cpp](https://github.com/ggerganov/llama.cpp) | C/C++ LLM inference, CPU/GPU / C/C++ 大模型推理，CPU/GPU | ![Stars](https://img.shields.io/github/stars/ggerganov/llama.cpp) |
| [TGI](https://github.com/huggingface/text-generation-inference) | Hugging Face's production serving / Hugging Face 生产级服务 | ![Stars](https://img.shields.io/github/stars/huggingface/text-generation-inference) |
| [SGLang](https://github.com/sgl-project/sglang) | Fast structured generation for LLMs / 快速结构化生成 | ![Stars](https://img.shields.io/github/stars/sgl-project/sglang) |
| [TensorRT-LLM](https://github.com/NVIDIA/TensorRT-LLM) | NVIDIA optimized inference / NVIDIA 优化推理 | ![Stars](https://img.shields.io/github/stars/NVIDIA/TensorRT-LLM) |
| [LMDeploy](https://github.com/InternLM/lmdeploy) | Efficient LLM deployment toolkit / 高效大模型部署工具 | ![Stars](https://img.shields.io/github/stars/InternLM/lmdeploy) |
| [LocalAI](https://github.com/mudler/LocalAI) | OpenAI-compatible local API / OpenAI 兼容本地 API | ![Stars](https://img.shields.io/github/stars/mudler/LocalAI) |
| [LM Studio](https://lmstudio.ai/) | GUI for local LLM inference / 本地大模型推理 GUI | — |
| [Jan](https://github.com/janhq/jan) | Open-source ChatGPT alternative, local / 开源本地 ChatGPT 替代 | ![Stars](https://img.shields.io/github/stars/janhq/jan) |
| [ExLlamaV2](https://github.com/turboderp/exllamav2) | Optimized GPTQ/EXL2 inference / 优化 GPTQ/EXL2 推理 | ![Stars](https://img.shields.io/github/stars/turboderp/exllamav2) |
| [MLC-LLM](https://github.com/mlc-ai/mlc-llm) | Universal LLM deployment on any device / 任意设备通用大模型部署 | ![Stars](https://img.shields.io/github/stars/mlc-ai/mlc-llm) |
| [OpenRouter](https://openrouter.ai/) | Unified API for 200+ models / 200+ 模型统一 API | — |

---

## Fine-Tuning & Training / 微调与训练

> Tools and frameworks for training and adapting LLMs / 训练与适配大模型的工具和框架

| Tool / 工具 | Description / 描述 | Stars |
|---|---|---|
| [Unsloth](https://github.com/unslothai/unsloth) | 2-5x faster fine-tuning, 80% less VRAM / 2-5倍快速微调，80% 更少显存 | ![Stars](https://img.shields.io/github/stars/unslothai/unsloth) |
| [Axolotl](https://github.com/axolotl-ai-cloud/axolotl) | Streamlined LLM fine-tuning / 简化大模型微调 | ![Stars](https://img.shields.io/github/stars/axolotl-ai-cloud/axolotl) |
| [LLaMA-Factory](https://github.com/hiyouga/LLaMA-Factory) | Easy fine-tuning for 100+ LLMs, WebUI / 100+ 大模型简易微调，WebUI | ![Stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Factory) |
| [PEFT](https://github.com/huggingface/peft) | Parameter-efficient fine-tuning (LoRA, etc.) / 参数高效微调(LoRA 等) | ![Stars](https://img.shields.io/github/stars/huggingface/peft) |
| [TRL](https://github.com/huggingface/trl) | RLHF/DPO training for transformers / Transformer RLHF/DPO 训练 | ![Stars](https://img.shields.io/github/stars/huggingface/trl) |
| [DeepSpeed](https://github.com/microsoft/DeepSpeed) | Microsoft's distributed training library / 微软分布式训练库 | ![Stars](https://img.shields.io/github/stars/microsoft/DeepSpeed) |
| [Megatron-LM](https://github.com/NVIDIA/Megatron-LM) | NVIDIA's large-scale training framework / NVIDIA 大规模训练框架 | ![Stars](https://img.shields.io/github/stars/NVIDIA/Megatron-LM) |
| [torchtune](https://github.com/pytorch/torchtune) | PyTorch native LLM fine-tuning / PyTorch 原生大模型微调 | ![Stars](https://img.shields.io/github/stars/pytorch/torchtune) |
| [SWIFT](https://github.com/modelscope/swift) | ModelScope LLM training & inference / 魔搭大模型训练与推理 | ![Stars](https://img.shields.io/github/stars/modelscope/swift) |
| [OpenRLHF](https://github.com/OpenRLHF/OpenRLHF) | High-performance RLHF framework / 高性能 RLHF 框架 | ![Stars](https://img.shields.io/github/stars/OpenRLHF/OpenRLHF) |
| [Transformers](https://github.com/huggingface/transformers) | The foundation library for LLMs / 大模型基础库 | ![Stars](https://img.shields.io/github/stars/huggingface/transformers) |

---

## Evaluation & Benchmarks / 评测与基准测试

> Leaderboards, benchmarks, and evaluation tools / 排行榜、基准测试与评估工具

### Leaderboards / 排行榜

| Leaderboard / 排行榜 | Description / 描述 | Link / 链接 |
|---|---|---|
| Arena (LMSYS Chatbot Arena) | Crowdsourced Elo ratings, 6M+ votes / 众包 Elo 评分，600万+ 投票 | [arena.ai](https://arena.ai/) |
| Open LLM Leaderboard | Hugging Face open model rankings / Hugging Face 开源模型排名 | [HF Leaderboard](https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard) |
| MTEB Leaderboard | Embedding model rankings / 嵌入模型排名 | [HF MTEB](https://huggingface.co/spaces/mteb/leaderboard) |
| Artificial Analysis | Independent LLM quality + speed rankings / 独立大模型质量+速度排名 | [artificialanalysis.ai](https://artificialanalysis.ai/) |
| LiveCodeBench | Live coding benchmark / 实时编码基准 | [livecodebench.github.io](https://livecodebench.github.io/) |
| LLM-Stats | Comprehensive model tracker / 综合模型追踪器 | [llm-stats.com](https://llm-stats.com/) |

### Benchmarks / 基准测试

| Benchmark / 基准 | Focus / 侧重 | Description / 描述 |
|---|---|---|
| MMLU-Pro | Knowledge / 知识 | 14K multi-domain questions, harder MMLU / 14K 多领域问题，更难版 MMLU |
| GPQA Diamond | Science / 科学 | Graduate-level science QA / 研究生级科学问答 |
| AIME | Math / 数学 | Competition math problems / 竞赛数学题 |
| HumanEval / MBPP | Code / 代码 | Code generation correctness / 代码生成正确性 |
| SWE-bench | Software Eng / 软件工程 | Real GitHub issue resolution / 真实 GitHub 问题修复 |
| ARC-AGI v2 | Reasoning / 推理 | Fluid intelligence, AGI-oriented / 流体智力，AGI 导向 |
| Humanity's Last Exam | General / 综合 | Hardest human-curated questions / 最难人工策划问题 |
| IFBench | Instruction / 指令 | Instruction following accuracy / 指令遵循准确性 |
| Terminal-Bench | CLI / 命令行 | Terminal command generation / 终端命令生成 |
| τ²-Bench | Domain / 领域 | Telecom domain benchmark / 电信领域基准 |
| AlpacaEval | Chat / 对话 | LLM-as-judge evaluation / LLM-as-judge 评估 |
| MT-Bench | Multi-turn / 多轮 | Multi-turn conversation quality / 多轮对话质量 |
| C-Eval | Chinese / 中文 | Chinese knowledge evaluation / 中文知识评测 |
| CMMLU | Chinese / 中文 | Chinese MMLU equivalent / 中文版 MMLU |

### Evaluation Tools / 评估工具

| Tool / 工具 | Description / 描述 | Stars |
|---|---|---|
| [lm-evaluation-harness](https://github.com/EleutherAI/lm-evaluation-harness) | Standard LLM evaluation framework / 标准大模型评估框架 | ![Stars](https://img.shields.io/github/stars/EleutherAI/lm-evaluation-harness) |
| [OpenCompass](https://github.com/open-compass/opencompass) | Comprehensive LLM evaluation platform / 全面大模型评测平台 | ![Stars](https://img.shields.io/github/stars/open-compass/opencompass) |
| [HELM](https://github.com/stanford-crfm/helm) | Stanford holistic LLM evaluation / 斯坦福整体大模型评估 | ![Stars](https://img.shields.io/github/stars/stanford-crfm/helm) |
| [promptfoo](https://github.com/promptfoo/promptfoo) | LLM prompt testing & evaluation / 大模型提示词测试与评估 | ![Stars](https://img.shields.io/github/stars/promptfoo/promptfoo) |

---

## API Providers & Aggregators / API 提供商与聚合平台

> Services offering LLM API access / 提供大模型 API 访问的服务

### Direct Providers / 直接提供商

| Provider / 提供商 | Models / 模型 | Pricing Page / 价格页 |
|---|---|---|
| [OpenAI](https://platform.openai.com/) | GPT-5, GPT-4o, GPT-4.1, o3, o4-mini | [Pricing](https://openai.com/pricing) |
| [Anthropic](https://console.anthropic.com/) | Claude Opus/Sonnet/Haiku 4.5/4.6 | [Pricing](https://anthropic.com/pricing) |
| [Google AI](https://aistudio.google.dev/) | Gemini 3 Pro, 2.5 Flash/Pro | [Pricing](https://ai.google.dev/pricing) |
| [xAI](https://console.x.ai/) | Grok-3, Grok-3 Mini | [Pricing](https://x.ai/api) |
| [Mistral](https://console.mistral.ai/) | Mistral Large 3, Codestral, Nemo | [Pricing](https://mistral.ai/pricing) |
| [DeepSeek](https://platform.deepseek.com/) | DeepSeek-V3, R1, Coder | [Pricing](https://platform.deepseek.com/pricing) |
| [Cohere](https://dashboard.cohere.com/) | Command R+, Embed v4 | [Pricing](https://cohere.com/pricing) |
| [Moonshot](https://platform.moonshot.cn/) | Kimi K2, Kimi-Dev-72B | [Pricing](https://platform.moonshot.cn/pricing) |
| [Zhipu AI (智谱)](https://open.bigmodel.cn/) | GLM-4, CodeGeeX4 | [Pricing](https://open.bigmodel.cn/pricing) |
| [Baidu (百度)](https://cloud.baidu.com/product/wenxinworkshop) | ERNIE 4.5 | [Pricing](https://cloud.baidu.com/pricing) |
| [Alibaba Cloud (阿里云)](https://dashscope.aliyun.com/) | Qwen3, Qwen-VL, Qwen-Audio | [Pricing](https://dashscope.aliyun.com/) |
| [ByteDance (字节)](https://www.volcengine.com/product/doubao) | Doubao 1.5 Pro | [Pricing](https://www.volcengine.com/pricing) |
| [SiliconFlow (硅基流动)](https://siliconflow.cn/) | Multiple open models / 多种开源模型 | [Pricing](https://siliconflow.cn/pricing) |

### Aggregators & Routers / 聚合与路由

| Platform / 平台 | Description / 描述 |
|---|---|
| [OpenRouter](https://openrouter.ai/) | 200+ models, unified API, cheapest routing / 200+ 模型，统一 API，最低价路由 |
| [Together AI](https://www.together.ai/) | Fast open model inference + fine-tuning / 快速开源模型推理+微调 |
| [Groq](https://groq.com/) | Ultra-fast LPU inference / 超快 LPU 推理 |
| [Fireworks AI](https://fireworks.ai/) | Fast, affordable open model hosting / 快速实惠的开源模型托管 |
| [Replicate](https://replicate.com/) | Run open models via API / 通过 API 运行开源模型 |
| [Anyscale](https://www.anyscale.com/) | Scalable Ray-based inference / 基于 Ray 的可扩展推理 |
| [Cerebras](https://cerebras.ai/) | Wafer-scale chip, fastest inference / 晶圆级芯片，最快推理 |
| [SambaNova](https://sambanova.ai/) | Enterprise AI infrastructure / 企业 AI 基础设施 |
| [Novita AI](https://novita.ai/) | Affordable GPU cloud for LLMs / 实惠的大模型 GPU 云 |

### Pricing Trackers / 价格追踪

| Tool / 工具 | Description / 描述 |
|---|---|
| [PricePerToken](https://pricepertoken.com/) | Compare 300+ model costs / 比较 300+ 模型成本 |
| [LLM Price Check](https://llmpricecheck.com/) | Quick price comparison / 快速价格对比 |
| [CostGoat](https://costgoat.com/compare/llm-api) | Monthly updated pricing guide / 月度更新价格指南 |
| [Helicone Calculator](https://www.helicone.ai/llm-cost) | Usage-based cost calculator / 基于用量的成本计算器 |

---

## Learning Resources / 学习资源

> Courses, papers, and guides for understanding LLMs / 理解大模型的课程、论文与指南

### Awesome Lists / 精选列表

| Resource / 资源 | Description / 描述 | Stars |
|---|---|---|
| [Awesome-LLM](https://github.com/Hannibal046/Awesome-LLM) | Most comprehensive LLM resource list / 最全面的大模型资源列表 | ![Stars](https://img.shields.io/github/stars/Hannibal046/Awesome-LLM) |
| [Awesome-Efficient-LLM](https://github.com/horseee/Awesome-Efficient-LLM) | Compression, pruning, quantization / 压缩、剪枝、量化 | ![Stars](https://img.shields.io/github/stars/horseee/Awesome-Efficient-LLM) |
| [Awesome-LLM-Safety](https://github.com/ydyjya/Awesome-LLM-Safety) | Safety & alignment research / 安全与对齐研究 | ![Stars](https://img.shields.io/github/stars/ydyjya/Awesome-LLM-Safety) |
| [Awesome-LLM-RAG](https://github.com/jxzhangjhu/Awesome-LLM-RAG) | RAG techniques & papers / RAG 技术与论文 | ![Stars](https://img.shields.io/github/stars/jxzhangjhu/Awesome-LLM-RAG) |
| [Awesome-LLM-Interpretability](https://github.com/JShollaj/awesome-llm-interpretability) | Model interpretability research / 模型可解释性研究 | ![Stars](https://img.shields.io/github/stars/JShollaj/awesome-llm-interpretability) |
| [Awesome-LLM-Books](https://github.com/Jason2Brownlee/awesome-llm-books) | Curated LLM book list / 精选大模型书籍 | ![Stars](https://img.shields.io/github/stars/Jason2Brownlee/awesome-llm-books) |

### Courses / 课程

| Course / 课程 | Provider / 提供方 | Description / 描述 |
|---|---|---|
| [LLM101n](https://github.com/karpathy/LLM101n) | Andrej Karpathy | Build a Storyteller AI from scratch / 从零构建故事 AI |
| [LLM Course](https://github.com/mlabonne/llm-course) | Maxime Labonne | Roadmap to LLM mastery with resources / 大模型精通路线图 |
| [Generative AI for Beginners](https://github.com/microsoft/generative-ai-for-beginners) | Microsoft | 21-lesson course on GenAI / 21课时生成式AI课程 |
| [Full Stack LLM Bootcamp](https://fullstackdeeplearning.com/llm-bootcamp/) | FSDL | Practical LLM application building / 实用大模型应用构建 |
| [Practical Deep Learning](https://course.fast.ai/) | fast.ai | Hands-on deep learning with LLMs / 动手深度学习与大模型 |
| [Stanford CS324](https://stanford-cs324.github.io/winter2022/) | Stanford | Understanding LLMs / 理解大语言模型 |
| [Stanford CS229](https://cs229.stanford.edu/) | Stanford | Machine Learning fundamentals / 机器学习基础 |
| [DeepLearning.AI Short Courses](https://www.deeplearning.ai/short-courses/) | DeepLearning.AI | LLM prompt engineering, fine-tuning, RAG / 提示工程、微调、RAG |
| [HuggingFace NLP Course](https://huggingface.co/learn/nlp-course/) | Hugging Face | NLP with Transformers / Transformers NLP |

### Key Papers / 重要论文

| Paper / 论文 | Year / 年份 | Description / 描述 |
|---|---|---|
| [Attention Is All You Need](https://arxiv.org/abs/1706.03762) | 2017 | The Transformer architecture / Transformer 架构 |
| [BERT](https://arxiv.org/abs/1810.04805) | 2018 | Bidirectional pre-training / 双向预训练 |
| [GPT-2](https://cdn.openai.com/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) | 2019 | Unsupervised multitask learning / 无监督多任务学习 |
| [Scaling Laws for Neural LMs](https://arxiv.org/abs/2001.08361) | 2020 | Kaplan et al. scaling laws / Kaplan 等人的缩放定律 |
| [GPT-3](https://arxiv.org/abs/2005.14165) | 2020 | Few-shot learning at scale / 大规模少样本学习 |
| [Training Compute-Optimal LMs](https://arxiv.org/abs/2203.15556) | 2022 | Chinchilla scaling laws / Chinchilla 缩放定律 |
| [LLaMA](https://arxiv.org/abs/2302.13971) | 2023 | Open foundation models / 开放基础模型 |
| [Constitutional AI](https://arxiv.org/abs/2212.08073) | 2022 | Anthropic's alignment approach / Anthropic 的对齐方法 |
| [RLHF](https://arxiv.org/abs/2203.02155) | 2022 | Training LMs with human feedback / 人类反馈训练语言模型 |
| [LoRA](https://arxiv.org/abs/2106.09685) | 2021 | Low-rank adaptation for LLMs / 大模型低秩适配 |
| [Chain-of-Thought Prompting](https://arxiv.org/abs/2201.11903) | 2022 | Reasoning via intermediate steps / 通过中间步骤推理 |
| [Mixture-of-Experts](https://arxiv.org/abs/2401.04088) | 2024 | DeepSeekMoE efficient scaling / DeepSeekMoE 高效扩展 |
| [DeepSeek-R1](https://arxiv.org/abs/2501.12948) | 2025 | RL-based reasoning without SFT / 无需 SFT 的 RL 推理 |
| [Qwen Technical Report](https://arxiv.org/abs/2309.16609) | 2023 | Qwen architecture & training / Qwen 架构与训练 |
| [LLM Evolution 2019-2026](https://www.llm-evolution.com/) | 2026 | 244 model reference / 244 模型参考 |

### Model Hubs / 模型中心

| Hub / 平台 | Description / 描述 |
|---|---|
| [Hugging Face](https://huggingface.co/models) | Largest open model hub, 900K+ models / 最大开源模型中心，90万+ 模型 |
| [ModelScope (魔搭)](https://modelscope.cn/) | Alibaba's model hub, strong in Chinese models / 阿里模型中心，中文模型丰富 |
| [Kaggle Models](https://www.kaggle.com/models) | Google-backed model repository / 谷歌支持的模型仓库 |
| [NVIDIA NGC](https://catalog.ngc.nvidia.com/) | NVIDIA optimized model catalog / NVIDIA 优化模型目录 |

---

## Contributing / 贡献指南

Contributions are welcome! Please read our **[Contributing Guide](CONTRIBUTING.md)** for details.

欢迎贡献！请阅读 **[贡献指南](CONTRIBUTING.md)** 了解详情。

**Quick summary / 快速摘要:**

1. **Fork** this repository / Fork 本仓库
2. Add your entry in the **correct category** and **alphabetical order** / 在正确分类中按字母顺序添加条目
3. Follow the bilingual format: `English / 中文` / 遵循中英文对照格式
4. Submit a **Pull Request** with a clear description / 提交带有清晰描述的 PR

### Format / 格式

```markdown
| [Model Name](https://link) | Description / 描述 | ![Stars](https://img.shields.io/github/stars/owner/repo) |
```

### Quality Standards / 质量标准

- No duplicates / 不重复
- No broken links / 无失效链接
- Actively maintained (commit within 6 months) / 积极维护（6个月内有提交）
- For open-source models: include GitHub stars badge / 开源模型需包含 GitHub 星标

---

## License / 许可

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

This list is released under CC0. / 本列表以 CC0 协议发布。
