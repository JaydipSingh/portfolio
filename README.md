# 📌 Jaydip Singh - Portfolio

Welcome to my professional portfolio! Here you'll find highlights of my key projects showcasing expertise in **systems programming**, **machine learning infrastructure**, and **research-aligned software engineering**.

---

## Featured Projects

### [Subword Tokenizer: BPE in Rust + Python](https://github.com/upcomingtrillioner12-design/subword_tokenizer)
**Small Language Model (SLM) Foundation Framework**

A production-ready tokenization and prototype training framework for efficient language models, built with cutting-edge 2026 research alignment.

**Key Contributions:**
- Built high-performance Rust BPE tokenizer (32K vocab, <4ms inference)
- Implemented Python prototype trainer with arXiv streaming + MPS support
- Designed checkpoint auto-ranking system for multi-run validation
- Research-aligned with 2026 SLM efficiency trends (LoRA, distillation, on-device)
- Added resilience layer: exponential backoff retry + streaming timeout handling (100+ retries)

**Technical Highlights:**
- **Tech Stack**: Rust, Python, PyTorch, CI/CD automation, Apple Metal Performance Shaders (MPS)
- **Key Metrics**: 35.2M param TinyLM model, 3-4h training on Apple Silicon M3 Pro, <2 sec/step inference
- **Architecture**: End-to-end pipeline (arXiv → streaming → tokenization → training → evaluation)
- **Robustness**: Multi-run checkpoint comparison, automatic best model selection, graceful degradation

**Research Context:**
Aligned with frontier SLM research (June-July 2026):
- The Wiola Architecture for Efficient SLMs
- CHERRY: Compressed Hierarchical Experts
- Continual Learning for Sequential Personalization
- Resource-Aware Neuro-Symbolic Reasoning for Local SLMs

**Roadmap Phases:**
- ✅ Phase 1: Prototype 35M-param TinyLM on physics corpus (complete)
- 🔄 Phase 2: LoRA fine-tuning, offline dataset training (in progress)
- 📋 Phase 3: RAG integration with knowledge base
- 📋 Phase 4+: Quantization, distillation, on-device benchmarking, agent framework

**Resources:**
- [Full README](https://github.com/upcomingtrillioner12-design/subword_tokenizer)
- [Architecture Documentation](https://github.com/upcomingtrillioner12-design/subword_tokenizer/blob/main/doc/architecture.md)
- [Project Reference](https://github.com/upcomingtrillioner12-design/subword_tokenizer/blob/main/doc/project_reference.md)
- [GitHub Repository](https://github.com/upcomingtrillioner12-design/subword_tokenizer)

### [Agentic Video Generator (Multi-Agent Video Pipeline)](https://github.com/JaydipSingh/agentic-video-generator)
**End-to-End Agentic Media Generation Platform**

A production-style multi-agent application that converts story prompts into generated videos using a checkpointed LangGraph pipeline, async job processing, and modular provider adapters.
**Key Contributions:**
- Architected a 6-node LangGraph workflow (director -> storyboard -> asset_generator -> voice -> editor -> critic)
- Implemented durable checkpointing with Postgres + Redis cache and resume endpoint (POST /jobs/{job_id}/resume)
- Built FastAPI backend with queue-backed asynchronous execution and job status polling
- Added dual frontend support: Streamlit UI and modern React UI with auto-polling, resume action, and video preview
- Integrated ffmpeg rendering pipeline with scene composition, concat workflow, and narration muxing
**Technical Highlights:**
- **Tech Stack**: FastAPI, LangGraph, SQLAlchemy, Redis, Postgres, ffmpeg, Streamlit, React, Tailwind CSS
- **Resilience**: Node-level checkpoints, resume routing, fallback providers for offline-safe execution
- **Architecture**: API + worker + queue + provider abstraction + rendering pipeline + UI parity across Python/React
- **Documentation**: Mermaid architecture diagrams + LaTeX status report with generated PDF
**Resources:**
- [GitHub Repository](https://github.com/JaydipSingh/agentic-video-generator)
- [Portfolio Repository](https://github.com/JaydipSingh/portfolio)

---

## Skills & Technologies

**Languages:** Rust, Python, C++, JavaScript/TypeScript  
**ML/AI:** PyTorch, TensorFlow, arXiv API, Model training & evaluation, Checkpoint management  
**Systems:** Cargo, Git, CI/CD (GitHub Actions), Shell scripting, Cross-platform development  
**Apple Silicon:** MPS (Metal Performance Shaders), M3 Pro optimization  
**Research:** Literature review, arXiv mining, SLM alignment, Efficiency-first design  

---

## About Me

I'm a software engineer focused on building efficient, research-aligned ML infrastructure. My work emphasizes:
- **Quality**: Production-ready code with comprehensive testing and documentation
- **Efficiency**: Optimized for resource-constrained environments (edge, mobile, embedded)
- **Research Currency**: Aligned with frontier directions in small language models and on-device AI
- **Robustness**: Defensive programming for long-running unattended workflows

---

## Let's Connect

- **GitHub**: [upcomingtrillioner12-design](https://github.com/upcomingtrillioner12-design)
- **Email**: jaydip.singh@gmail.com  
- **LinkedIn**: [Jaydip Singh](https://www.linkedin.com/in/jaydip-singh-15714546/)

---

**Last Updated:** July 10, 2026
