# 👋 Hi, I'm Hongping Zhang

Independent AI Researcher | Energy Efficiency & Sustainable Computing
## 🚀 Core Assets

| Asset | Type | Impact | Link |
|-------|------|--------|------|
| **🤗 HuggingFace Optimum Integration** | Official Documentation | Trusted by thousands of HF developers | [View Docs →](https://huggingface.co/docs/optimum/concept_guides/quantization) |
| **📊 Complete Energy Dataset** | Research Benchmark | 113+ configurations, 5 precision methods | [Explore Data →](https://huggingface.co/datasets/hongpingzhang/ecocompute-energy-efficiency) |
| **🦞 EcoCompute AI Assistant** | Interactive Tool | Conversational energy advisor on ClawHub | [Try EcoCompute →](https://clawhub.ai/hongping-zh/ecocompute) |

### Key Discoveries
- 🔥 **FP8 Paradox**: +701% energy overhead on RTX 5090 (torchao confirmed)
- ⚡ **Small-Model Paradox**: +25-56% energy penalty for NF4 <3B models  
- 📈 **Batch Size Impact**: 95.7% energy reduction (BS=1→64) on A800

---
---

## 🔬 Research Highlights

### 🏆 Energy Efficiency of Quantized LLM Inference

**[Paper (Draft)](https://github.com/hongping-zh/ecocompute-dynamic-eval) | [Dashboard](https://hongping-zh.github.io/ecocompute-dynamic-eval/) | [Batch Size Analysis](https://hongping-zh.github.io/ecocompute-dynamic-eval/?view=BATCH_SIZE) | [Metadata](https://github.com/hongping-zh/ecocompute-dynamic-eval/tree/main/metadata)**

> **Breakthrough Finding**: Discovered that bitsandbytes INT8 increases energy by 17-147% due to mixed-precision decomposition. Causal diagnosis via ablation recovered **+79-98% throughput** and **−35-41% energy** across consumer (RTX 4090D) and datacenter (A800) GPUs.

> **NEW — Batch Size Optimization**: A800 sweep (BS 1→64) shows **95.7% energy reduction** and **55.5× throughput scaling**. BS=1 wastes 55% GPU capacity. Interactive results: [**View Dashboard →**](https://hongping-zh.github.io/ecocompute-dynamic-eval/?view=BATCH_SIZE)

> **Research Scope**: This work focuses on energy efficiency diagnosis. Accuracy assessment (perplexity, downstream tasks) is not yet complete. Pure INT8 (`threshold=0.0`) shows major performance gains, but accuracy impact requires validation. Next steps: PPL and MMLU evaluation—contributions welcome!

**Key Contributions**:
- 🎯 **Root cause identified**: Mixed-precision decomposition, not INT8 itself
- 📊 **93+ measurements** (CV < 1-2%) across **3 GPU architectures**: RTX 5090 (Blackwell), RTX 4090D (Ada Lovelace), A800 (Ampere)
- 📈 **Batch size scaling law**: 95.7% energy reduction (BS=1→64), validated on A800 with 70 measurements
- ✅ **Cross-platform validation**: Consistent results across consumer & datacenter GPUs, multiple models
- 🔓 **Full reproducibility**: Complete metadata with software versions, configs, and protocols
- 🌐 **Open data**: All raw data, scripts, interactive dashboard, and provenance publicly available

**Impact**: Prevents industry from drawing wrong conclusions about INT8 quantization. Provides actionable guidance for practitioners deploying quantized LLMs in production.

**Status**: Preparing for arXiv submission. bitsandbytes Issues filed: [#1851 (NF4)](https://github.com/bitsandbytes-foundation/bitsandbytes/issues/1851) | [#1867 (INT8 Energy)](https://github.com/bitsandbytes-foundation/bitsandbytes/issues/1867)

---

## 📊 Research Standards

All my benchmarks follow rigorous reproducibility standards:

- ✅ **Complete metadata** with hardware specs, software versions, and model commits
- ✅ **Statistical rigor** (n=10, CV < 2%, significance tests)
- ✅ **Open data** with full provenance and reproducible scripts
- ✅ **Causal analysis** via controlled experiments and ablations
- ✅ **Cross-architecture validation** (Blackwell + Ada Lovelace + Ampere)

📁 **[View Metadata Standards →](https://github.com/hongping-zh/ecocompute-dynamic-eval/tree/main/metadata)**

---

## 🛠️ Tech Stack

**Languages**: Python, TypeScript, Bash  
**ML/AI**: PyTorch, Transformers, bitsandbytes, CUDA  
**Data**: Pandas, NumPy, SciPy, Matplotlib  
**Tools**: Git, Docker, Jupyter, VS Code  
**Cloud**: AutoDL, AWS (occasional)

---

## 📈 Current Projects

### 🌱 EcoCompute Dynamic Eval
Interactive dashboard for comparing AI models by accuracy, cost, and carbon footprint. Features a **[Batch Size Analysis page](https://hongping-zh.github.io/ecocompute-dynamic-eval/?view=BATCH_SIZE)** with interactive charts and cost calculator.

**Tech**: TypeScript, React, Recharts, TailwindCSS, GitHub Pages  
**Data**: 93+ measurements, 8 models, 3 GPU architectures (RTX 5090, RTX 4090D, A800)

### 🔋 Quantization Energy Research
Systematic study of quantization energy efficiency on modern GPUs. Discovered two paradoxes (NF4 and bitsandbytes INT8) and provided causal diagnosis via ablation. Latest: **batch size sweep reveals 95.7% energy reduction** potential.

**Tech**: Python, PyTorch, NVML, bitsandbytes  
**Impact**: Prevents ~30-96% energy waste in production LLM deployments

---

## 📫 Contact

- **Email**: zhanghongping1982@gmail.com
- **GitHub**: [@hongping-zh](https://github.com/hongping-zh)
- **Dashboard**: [ecocompute-dynamic-eval](https://hongping-zh.github.io/ecocompute-dynamic-eval/)

---

## 💡 Philosophy

I believe in **open science** and **reproducible research**. Every benchmark I publish includes:
- Complete metadata (hardware, software, models)
- Raw data and analysis scripts
- Reproduction commands
- Known issues and resolutions

**Goal**: Make AI research more transparent, reproducible, and energy-efficient.

---

## 📊 GitHub Stats

[![Hongping's GitHub stats](https://github-readme-stats.vercel.app/api?username=hongping-zh&show_icons=true&theme=default&cache_seconds=1800)](https://github.com/hongping-zh)

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=hongping-zh&layout=compact&theme=default&cache_seconds=1800)](https://github.com/hongping-zh)

[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=hongping-zh&theme=default)](https://github.com/hongping-zh)

---

*"Measure, don't assume. Reproduce, don't trust. Share, don't hoard."*
