<p align="center">
  <img src="./assets/profile-banner.jpg" alt="cluster1900 banner" width="100%" />
</p>

# Hi，我是 Hawk Wu 👋

**写中文 LLM / AI 工程教程，也做实用的 Agent 与 Coding Agent。**
*Chinese-language LLM & AI-engineering tutorials · building practical agents.*

我把读源码、训模型、做 Agent 的过程整理成**能跑、能验证**的中文教程：从高中数学讲到 Transformer，从 vLLM / MiniMind 源码讲到自己动手预训练。之前长期做后端与分布式系统、交易所和多链钱包基础设施，现在专注 AI 工程。

[![Website](https://img.shields.io/badge/Blog-apexolab.com-0A66C2?style=flat-square)](https://apexolab.com)
[![X](https://img.shields.io/badge/X-@Wu005887-111111?style=flat-square&logo=x)](https://x.com/Wu005887)

## 📚 教程与项目索引

### 从零学 AI

| 项目 | 简介 |
| --- | --- |
| [ai-engineering-from-scratch-zh](https://github.com/cluster1900/ai-engineering-from-scratch-zh) · [网站](https://ai-learn.apexolab.com/) | 《AI Engineering from Scratch》中文版：20 个阶段、500+ 节课，从线性代数一路到 Agent 与 MCP |
| [zero2llm](https://github.com/cluster1900/zero2llm) · [在线阅读](https://cluster1900.github.io/zero2llm/) | 写给初学者的 Transformer：高中数学 + 逐行 PyTorch，亲手训练一个 Baby-GPT（含 EPUB） |
| [ai-engineering-interview-questions-CN](https://github.com/cluster1900/ai-engineering-interview-questions-CN) | AI / LLM / Agent 工程师中文面试题与参考答案：RAG、Agent、微调、LLMOps、系统设计 |

### 源码阅读

| 项目 | 简介 |
| --- | --- |
| [vllm_reader](https://github.com/cluster1900/vllm_reader) · [在线阅读](https://cluster1900.github.io/vllm_reader/) | vLLM V1 源码图文教程：请求生命周期、调度与 Continuous Batching、KV Cache、PagedAttention、分布式推理 |
| [minimind_reader](https://github.com/cluster1900/minimind_reader) · [在线阅读](https://cluster1900.github.io/minimind_reader/) | 从零读懂大模型：MiniMind / MiniMind-V / MiniMind-O 源码精读，20 章，附 EPUB / PDF 与 CPU 实验 |

### 动手训练与 Agent

| 项目 | 简介 |
| --- | --- |
| [pretraining-a-mini-kimi-k3](https://github.com/cluster1900/pretraining-a-mini-kimi-k3) | 正在从 0 训练的约 1.15B 参数（激活约 0.16B）Kimi-K3 风格 MoE 模型：KDA + MLA 混合注意力，4×V100 分布式预训练（训练中） |
| [lora-asr](https://github.com/cluster1900/lora-asr) | 基于 Qwen3-ASR-1.7B 的鲁棒语音识别后训练：SFT → DPO → RL，中英文 WER/CER 评测 |
| [opencode-rs](https://github.com/cluster1900/opencode-rs) | 用 Rust 重写 opencode：可审计、可测试的 Coding Agent 内核（重构中） |

## 🔭 最近在做

- 小型 Kimi-K3 风格模型的数据准备与分布式预训练，过程会整理成教程
- Rust Coding Agent 的 harness、工具调用与评测
- 昇腾 NPU 上的大模型推理部署（Prefill/Decode 分离对比）

## 📫 联系我

- 博客：[apexolab.com](https://apexolab.com)
- X：[@Wu005887](https://x.com/Wu005887)
- 教程有错误或想看的主题，欢迎直接提 Issue；觉得有用的话点个 ⭐ 就是最大的支持。
