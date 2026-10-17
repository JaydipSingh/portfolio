# 📌 Jaydip Singh — Portfolio

Welcome to my professional portfolio. Here you'll find highlights of my key
projects spanning **machine learning research**, **small/efficient language
models**, **multimodal AI**, and **agentic systems**.

---

## Featured Projects

### [SLM Physics Assistant: Domain-Specialized Small Language Model](https://github.com/JaydipSingh/slm-physics-assistant)
**A reproducible stack for training domain-specialized SLMs on a laptop**

A complete, open-source pipeline — Rust BPE tokenizer, custom PyTorch transformer,
LoRA fine-tuning, and a multi-metric evaluation harness — that trains a
physics-specialized small language model end-to-end on a single Apple M3 Pro
(18 GB). Accompanied by a research paper (preprint; arXiv ID forthcoming).

**Key results:**
- A **23M-parameter** physics model scores **0.55** on a multiple-choice physics
  QA benchmark, **outperforming GPT-2 Large (774M) by 69%** despite being 33× smaller.
- Documented and fixed a practical training failure mode (early end-of-sequence
  collapse) via EOS-free document packing.

**Technical highlights:**
- **Tech stack:** Rust, Python, PyTorch, Apple Metal Performance Shaders (MPS)
- **Architecture:** custom decoder-only transformer (RoPE, RMSNorm, SwiGLU) with
  explicit Q/K/V/O projections for LoRA
- **Engineering:** live arXiv streaming with exponential-backoff retries,
  periodic checkpointing, automated tests + CI
- **License:** MIT

**Resources:** [GitHub Repository](https://github.com/JaydipSingh/slm-physics-assistant)

---

### [PhysVision-SLM: Multimodal Medical-Physics Visual QA](https://github.com/JaydipSingh/physvision-slm)
**Training multimodal SLMs on simulation-generated data (no human annotation)**

A multimodal small language model that answers questions about simulated medical
physics images (PET reconstructions, sinograms, phantom diagrams). An analytical
image simulator acts as a **zero-cost labeled-data generator** — every image
comes with exact ground truth, converted automatically into QA pairs.
Accompanied by a research paper (preprint; arXiv ID forthcoming).

**Key results:**
- A frozen **SigLIP + Qwen2-0.5B** configuration reaches **89.0%** on a
  35,596-pair visual-QA benchmark (vs. 25% random, 33% image-agnostic baseline).
- A compact 23M "lite" configuration reaches 43.7%; the controlled comparison
  attributes the gap primarily to the vision encoder.
- A pretrained encoder lifts fine spatial localization from below random (16%) to
  69%, with everything else held fixed.

**Technical highlights:**
- **Tech stack:** PyTorch, SigLIP, Qwen2, Hugging Face Transformers, MPS
- **Architecture:** vision encoder → learned projection → frozen language model
  (LLaVA-style alignment); only a ~4.8M-parameter connector is trained
- **Engineering:** simulation-based dataset generator, two-stage training,
  log-probability-ranking evaluation, diagnostic/vision-pathway checks
- **License:** MIT

**Resources:** [GitHub Repository](https://github.com/JaydipSingh/physvision-slm)

---

### [Agentic Video Generator (Multi-Agent Video Pipeline)](https://github.com/JaydipSingh/agentic-video-generator)
**End-to-end agentic media generation platform**

A production-style multi-agent application that converts story prompts into
generated videos using a checkpointed LangGraph pipeline, async job processing,
and modular provider adapters.

**Key contributions:**
- Architected a 6-node LangGraph workflow (director → storyboard →
  asset_generator → voice → editor → critic)
- Implemented durable checkpointing with Postgres + Redis and a resume endpoint
  (`POST /jobs/{job_id}/resume`)
- Built a FastAPI backend with queue-backed asynchronous execution and job-status
  polling
- Delivered dual frontends: a Streamlit UI and a React UI with auto-polling,
  resume, and video preview
- Integrated an ffmpeg rendering pipeline (scene composition, concat, narration muxing)

**Tech stack:** FastAPI, LangGraph, SQLAlchemy, Redis, Postgres, ffmpeg,
Streamlit, React, Tailwind CSS

**Resources:** [GitHub Repository](https://github.com/JaydipSingh/agentic-video-generator)

---

## Skills & Technologies

**Languages:** Python, Rust, C/C++, JavaScript/TypeScript, SQL
**ML/AI:** PyTorch, Hugging Face Transformers, LLMs, multimodal models, LoRA /
parameter-efficient fine-tuning, RAG, model training & evaluation
**Agentic AI:** LangGraph, LangChain, OpenAI Agents SDK, CrewAI, AutoGen, MCP
**Systems:** Git, GitHub Actions (CI/CD), Docker, shell scripting, cross-platform
development, Apple Silicon (MPS)
**Research:** literature review, reproducible experimentation, scientific computing,
Monte Carlo simulation (GEANT4)

---

## About Me

I'm a Ph.D.-qualified machine learning scientist working on agentic and
generative AI, with a research background in particle physics and scientific
computing. My recent independent work focuses on efficient, reproducible small
and multimodal language models that run on constrained hardware. I value:
- **Reproducibility:** tested, documented, end-to-end pipelines
- **Efficiency:** strong results on resource-constrained hardware
- **Honesty:** transparent reporting, including failure modes and limitations

---

## Let's Connect

- **GitHub:** [JaydipSingh](https://github.com/JaydipSingh)
- **Email:** jaydip.singh@gmail.com
- **LinkedIn:** [Jaydip Singh](https://www.linkedin.com/in/jaydip-singh-15714546/)
- **Research Profile:** [inspirehep.net](https://inspirehep.net/authors/1591917)

---

**Last Updated:** October 2026
