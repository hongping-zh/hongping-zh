# 👋 Hi, I'm Hongping

**Solo Founder of [EcoCompute AI](https://hongping-zh.github.io/ecocompute-dynamic-eval/) — the open-source decision engine for Sustainable AI Infrastructure.**

[![Live Demo](https://img.shields.io/badge/Live_Demo-Try_Now-brightgreen?style=for-the-badge)](https://hongping-zh.github.io/ecocompute-dynamic-eval/)
[![GitHub Stars](https://img.shields.io/github/stars/hongping-zh/ecocompute-dynamic-eval?style=for-the-badge&logo=github)](https://github.com/hongping-zh/ecocompute-dynamic-eval)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](https://github.com/hongping-zh/ecocompute-dynamic-eval/blob/main/LICENSE)

---

## 🌱 Mission

> **Green AI shouldn't be a luxury.** I'm building open-source tools that let engineers predict GPU cost and carbon impact *before* code merges — turning sustainability from an afterthought into a first-class engineering metric.

---

## 🔬 Key Research Finding

We benchmarked **8 models on NVIDIA RTX 5090 (Blackwell)** with NVML 10 Hz power sampling and discovered a counter-intuitive result:

| Model Size | FP16 vs NF4 | Energy Impact |
|------------|-------------|---------------|
| 1.1B TinyLlama | FP16 wins | NF4 uses **26.5% MORE** energy |
| 1.5B Qwen2 | FP16 wins | NF4 uses **29.4% MORE** energy |
| 3B Qwen2.5 | FP16 wins | NF4 uses **11.7% MORE** energy |
| 7B Qwen2 | **NF4 wins** | NF4 saves **11.4%** energy |

> **Insight**: 4-bit quantization only saves energy for models **>5B parameters**. For smaller models, FP16 is more efficient. This challenges the industry assumption that "quantization always saves energy."

---

## 🔥 Flagship Project

| | |
|---|---|
| **Project** | [**EcoCompute Dynamic Eval**](https://github.com/hongping-zh/ecocompute-dynamic-eval) |
| **Live Demo** | [hongping-zh.github.io/ecocompute-dynamic-eval](https://hongping-zh.github.io/ecocompute-dynamic-eval/) |
| **What it does** | Compare AI models by **Accuracy + Cost + Carbon** in one dashboard |
| **Status** | 🟢 Public Beta |
| **Stack** | React + TypeScript + Tailwind + Recharts |

### Core Features
- **Dynamic Leaderboard** with RTX 5090 verified benchmarks & provenance badges
- **Emissions Calculator** with 15+ templates, sensitivity analysis & break-even charts
- **DeepSeek vs GPT** workflow comparison
- **Paradox Visualization** — highlights when quantization *hurts* efficiency
- **Power Curve Detail** — per-model NVML 10 Hz sampling traces
- **Community Template Library** with GitHub Issue submission flow

---

## 🎯 2026 Roadmap

| Phase | Timeline | Milestone |
|-------|----------|-----------|
| **Phase 1** | ✅ Now | Open dashboard with RTX 5090 benchmarks, calculator, templates |
| **Phase 2** | Q2 2026 | VS Code Extension for real-time energy linting |
| **Phase 3** | Q3 2026 | REST API + continuous benchmark pipeline |
| **Phase 4** | Q4 2026 | ML-driven model routing engine for enterprise |

---

## 🤝 What I'm Looking For

- **Design Partners** — AI teams willing to pilot EcoCompute in their CI/CD pipeline
- **Open Source Contributors** — help expand benchmark coverage to more GPUs & models
- **Sponsors & Grants** — to accelerate development of the VS Code extension and API layer

---

## 📬 Let's Connect

- **Demo**: [hongping-zh.github.io/ecocompute-dynamic-eval](https://hongping-zh.github.io/ecocompute-dynamic-eval/)
- **Email**: zhanghongping1982@gmail.com
- **GitHub Sponsors**: [Sponsor this project](https://github.com/sponsors/hongping-zh)

> **If you're an investor, accelerator, or potential design partner** — I'd love to chat. Email me or open a Discussion on the repo.

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=hongping-zh&show_icons=true&theme=radical" alt="GitHub Stats" />
</p>
