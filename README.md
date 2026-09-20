<p align="center">
  <img src="./assets/profile-banner.jpg" alt="Hawk Wu AI systems workspace banner" width="100%" />
</p>

# Hawk Wu / cluster1900

**AI systems architect | LLM training and inference | Exchange and Web3 infrastructure**

I am a software architect and backend engineer with extensive experience building high-concurrency, high-availability products. I have worked across social and media platforms, healthcare IM, exchanges, multi-chain wallets, DEX infrastructure, distributed systems, coding agents, and applied AI.

I like difficult systems because they force the important questions into the open: what is the source of truth, what happens when a dependency fails, how do we observe the system, and can another engineer reproduce the result? My current work connects those questions across model training, model serving, agent products, and on-chain infrastructure.

[![Website](https://img.shields.io/badge/Website-agent--buy.com-0A66C2?style=flat-square)](https://agent-buy.com)
[![AI Learn](https://img.shields.io/badge/AI%20Learn-ai--learn.agent--buy.com-4C6FFF?style=flat-square)](https://ai-learn.agent-buy.com)
[![X](https://img.shields.io/badge/X-@Wu005887-111111?style=flat-square&logo=x)](https://x.com/Wu005887)
[![GitHub](https://img.shields.io/badge/GitHub-cluster1900-24292F?style=flat-square&logo=github)](https://github.com/cluster1900)

## What I am building now

- **[Kimi K3 / DeepSeek-style 1B model training](https://github.com/cluster1900/pretraining-a-mini-kimi-k3/tree/main/train)**: an ongoing training engineering project. The `train/` workspace implements KDA and MLA attention, routed MoE layers, KV-cache paths, fused kernels, a 4× Tesla V100 FP16/NCCL runner, WSD scheduling, MoE load balancing, telemetry, loss-spike protection, atomic checkpoint recovery, validation, and profiling. Its data pipeline records source and license provenance, converts and cleans heterogeneous corpora, performs exact and near deduplication plus 13-gram decontamination, verifies tokenizer equivalence, writes uint32 shards, audits manifests, and runs real-data smoke tests. Current work is finishing verified data preparation and distributed pretraining readiness, followed by alignment and long-context evaluation.
- **[vllm_reader](https://github.com/cluster1900/vllm_reader)**: source-level research and runnable experiments for vLLM V1, covering request lifecycle, Engine and EngineCore, scheduling and continuous batching, KV cache and PagedAttention, model execution, async execution and CUDA Graphs, distributed inference, and performance analysis. The [documentation site](https://cluster1900.github.io/vllm_reader/) provides the reading path and rendered examples.
- **LLM inference infrastructure**: deploying Qwen3.6-35B-A3B FP16 on Ascend NPUs, comparing monolithic and disaggregated Prefill/Decode serving with K3s, GitOps, observability, and benchmarks.
- **Coding Agent**: developing a practical Rust-based agent harness and exploring tools, memory, context management, evaluation, and reliable execution workflows.
- **Robust speech recognition**: working with Qwen3 1.7B ASR, baseline inference, WER/CER evaluation, LoRA, and routing experiments.
- **Deriw**: building an AI-operable decentralized perpetual exchange on a dedicated Ethereum L3, spanning smart contracts, cross-chain flows, trading infrastructure, and agent skills.
- **Sports AI**: private product work combining agents, sports data, analysis, and user-facing intelligence.

## Selected work

| Project | What it explores | Stack |
| --- | --- | --- |
| [pretraining-a-mini-kimi-k3](https://github.com/cluster1900/pretraining-a-mini-kimi-k3) | Training code, auditable data preparation, distributed pretraining, profiling, and evaluation | Python, PyTorch, CUDA, NCCL |
| [vllm_reader](https://github.com/cluster1900/vllm_reader) · [docs](https://cluster1900.github.io/vllm_reader/) | vLLM V1 source architecture, request scheduling, KV cache, execution, distributed inference, and performance experiments | Python, PyTorch, vLLM, CUDA |
| [Deriw](https://github.com/deriwfi) | An AI-operable perpetual DEX, dedicated Ethereum L3, cross-chain flows, and on-chain trading skills | Solidity, Go, JavaScript |
| [APDEX](https://github.com/cluster1900/apdex) | An independently engineered multi-chain DEX backend and trading infrastructure project | Go, Node.js, Solana Anchor |
| [ai-engineering-from-scratch-zh](https://github.com/cluster1900/ai-engineering-from-scratch-zh) | A practical Chinese AI engineering course, from linear algebra to agent systems | Python, TypeScript, Rust, Julia |
| [opencode-rs](https://github.com/cluster1900/opencode-rs) | A Rust coding-agent harness focused on usable engineering workflows | Rust, LLM agents |
| [lora-asr](https://github.com/cluster1900/lora-asr) | Robust ASR based on Qwen3 1.7B, with an evaluation-first path toward LoRA and routing | Python, Transformers |
| [eip7702-fulldemo](https://github.com/cluster1900/eip7702-fulldemo) | A complete EIP-7702 gasless transaction demo | Solidity |
| [ai-engineering-interview-questions-CN](https://github.com/cluster1900/ai-engineering-interview-questions-CN) | Chinese AI engineering interview questions and answers | Markdown |

## Engineering track record

- **CoinW — blockchain and exchange infrastructure**: currently building wallet and on-chain services, including node access, chain data, transaction broadcasting, scanners, asset aggregation, market and coin services, gateway boundaries, signer integration, and reusable chain adapters.
- **Bitget and KuCoin Wallet platforms**: designed and operated multi-chain wallet capabilities across 100+ chains and 100+ DEXs, covering DEX aggregation, routing, Market Registry, EVM and UTXO parsing, signing, broadcasting, asset accuracy, retries, and operational alerts.
- **Chengdu Medlinker — senior engineer**: led architecture and platform work for healthcare IM, including nearly 300 services, service governance, automated delivery, and an IM system supporting 1M+ concurrent users and 1B+ persisted chat records.
- **Starmaker — Golang Expert**: built backend systems for social, audio, video, live-streaming, content distribution, media processing, gateways, monitoring, recommendation, and moderation.
- **Earlier roles**: developed high-concurrency services for social products, content and file platforms, business systems, monitoring, and security checks.

Across these roles I have designed and operated multi-chain wallet foundations, EVM and UTXO scanners, signing and broadcasting systems, cross-chain swap services, DEX aggregation, market data pipelines, certificate and domain automation, service-mesh platforms, and application-security tooling.

## How I work

- **Start from invariants**: define ownership, state transitions, failure modes, and acceptance checks before optimizing implementation details.
- **Keep data traceable**: record source, version, license, hashes, processing scripts, statistics, and evaluation boundaries when data influences a model or a product.
- **Make production behavior visible**: use metrics, logs, checkpoints, smoke tests, reproducible commands, and recovery paths so that a running process is not mistaken for a completed result.
- **Write for the next engineer**: keep architecture decisions, trade-offs, failed experiments, and operational procedures close to the code.

## Areas of depth

**AI and model systems**

LLM development, model training, MoE, MLA, KDA, tokenizer and data pipelines, coding agents, RAG, memory, tool use, evaluation loops, LoRA, ASR, inference serving, long-context experiments, and AI-native product workflows.

**Crypto and Web3**

Exchange systems, wallet infrastructure, EVM, UTXO, Solidity, DEX aggregation, perpetual markets, L3 rollups, account abstraction, gasless transactions, chain indexing, multi-chain assets, signing, broadcasting, and cross-chain execution.

**Distributed systems**

Go and Rust services, high-concurrency architecture, TCP/UDP/HTTP, Redis, MongoDB, MySQL, Elasticsearch, Kubernetes, K3s, service mesh, observability, CI/CD, GitOps, and AWS operations.

## Toolbox

**Languages and protocols**

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3176C6?style=flat-square&logo=typescript&logoColor=white)
![Solidity](https://img.shields.io/badge/Solidity-363636?style=flat-square&logo=solidity&logoColor=white)

**AI and model systems**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![Transformers](https://img.shields.io/badge/Transformers-FFD21E?style=flat-square)
![Qwen](https://img.shields.io/badge/Qwen-615CED?style=flat-square)
![LoRA / QLoRA](https://img.shields.io/badge/LoRA%20%2F%20QLoRA-0F9D8A?style=flat-square)
![LLM Agents](https://img.shields.io/badge/LLM%20Agents-FF6B35?style=flat-square)
![RAG](https://img.shields.io/badge/RAG-4C6FFF?style=flat-square)
![ASR](https://img.shields.io/badge/ASR-00897B?style=flat-square)
![Model Serving](https://img.shields.io/badge/Model%20Serving-6A5ACD?style=flat-square)
![Evaluation](https://img.shields.io/badge/Model%20Evaluation-D1495B?style=flat-square)

**Infrastructure and Web3**

![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![K3s](https://img.shields.io/badge/K3s-FFC61C?style=flat-square&logo=k3s&logoColor=black)
![Ascend NPU](https://img.shields.io/badge/Ascend%20NPU-C7000B?style=flat-square)
![Web3](https://img.shields.io/badge/Web3-7B2CBF?style=flat-square)

## Find me

- Website: [agent-buy.com](https://agent-buy.com)
- AI notes and courses: [ai-learn.agent-buy.com](https://ai-learn.agent-buy.com)
- X: [@Wu005887](https://x.com/Wu005887)
- GitHub: [github.com/cluster1900](https://github.com/cluster1900)
