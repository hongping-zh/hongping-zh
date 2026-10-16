# 👋 Hi, I'm Hongping Zhang

Independent AI Researcher | Energy Efficiency & Sustainable Computing

---

## 🎯 Core Assets

| Asset | Type | Impact | Link |
|-------|------|--------|------|
| 🤗 **HuggingFace Optimum Integration** | Official Documentation | Findings integrated into official quantization guide (dataset v1.1.0) | [View Docs →](https://huggingface.co/docs/optimum/) |
| 📊 **Complete Energy Dataset** | Research Benchmark | 360+ configurations, 5 precision methods | [Explore Data →](https://github.com/hongping-zh/ecocompute-ai) |
| 🦾 **EcoCompute AI Assistant** | Interactive Tool | Conversational energy advisor on ClawHub | [Try EcoCompute →](https://clawhub.ai/hongping-zh/ecocompute) |
| 🏛️ **MLCommons Power WG Discussion** | Industry Recognition | Invited to contribute to MLPerf power measurement standards | [View Discussion →](https://github.com/mlcommons/inference/issues/2558) |

---

## 🔬 Core Discovery

> **NF4 crossover ranges from ~1.8B (Blackwell, current stack) to ~3.7B (Ada).**  
> Below the crossover, quantization costs more energy; above it, quantization saves. The crossover belongs to a card+stack combination, not to an architecture.  
> — Measured on RTX 4090D, RTX 5090, A800 with NVML power sampling.

This finding challenges the default assumption that "quantize everything = green." Our benchmark data is open and reproducible.

**Key Findings:**
- **NF4 crossover**: ~2.1B (Turing T4) → ~3.7B (Ada 4090) → ~4.8B (Blackwell 5090 v1.1.0); ~1.8B on 5090 with a newer stack
- **INT8 (`load_in_8bit=True`)**: default increases energy +17–147% vs FP16; set `llm_int8_threshold=0.0` to recover +79% throughput and −36% energy
- **Below crossover**: NF4 adds 11–29% energy (Blackwell, small models)
- **Above crossover**: NF4 saves 8–35% energy (Ada, models ≥6B)

---

## 🚀 Try It Now

| | |
|---|---|
| **🌐 Live Demo** | [**EcoCompute Dashboard →**](https://hongping-zh.github.io/) |
| **📊 What it does** | Compare AI models by **Accuracy × Cost × Carbon** in one dashboard |
| **⚡ Data source** | Real GPU benchmarks — PyTorch 2.10 + CUDA 12.8, 10 runs per config |

---

## 📈 Recognition & Impact

| Achievement | Details |
|-------------|---------|
| **🤗 HuggingFace Official** | Quantization energy findings integrated into Optimum documentation |
| **🏛️ MLCommons Invited** | Contributing to MLPerf Power Working Group on quantization energy metrics |
| **📊 Open Dataset** | 360+ configurations across 4 GPU architectures (Turing, Ampere, Ada, Blackwell), CV < 2% |
| **🌍 Zenodo Archive** | Permanent DOI: [10.5281/zenodo.19647290](https://zenodo.org/records/19647290) (dataset v1.1.0) + [10.5281/zenodo.22037483](https://zenodo.org/records/22037483) (RTX 4090 deep dive) |
| **📝 Research Paper** | "When Does Quantization Save Energy?" — arXiv submission in progress |

---

## 🎯 2026 Roadmap

- ✅ **HuggingFace Integration** — Official documentation published
- ✅ **MLCommons Engagement** — Invited to Power Working Group
- 🔄 **arXiv Publication** — Seeking endorsement for cs.LG submission
- 🛡️ **VS Code Extension** — Real-time energy linting before code merges
- 🤝 **Enterprise Pilots** — Seeking design partners for carbon-aware CI/CD

---

## 💚 How You Can Help

I'm looking for **design partners**, **early adopters**, **arXiv endorsers**, and **grant sponsors** to take EcoCompute from research to production.

| Action | Link |
|--------|------|
| ⭐ **Star the repo** | [ecocompute-mlcube](https://github.com/hongping-zh/ecocompute-mlcube) |
| 🌐 **Try the demo** | [Live Dashboard →](https://hongping-zh.github.io/) |
| 📧 **arXiv Endorsement** | [Email me →](mailto:zhanghongping1982@gmail.com?subject=arXiv%20Endorsement) |
| 🤝 **Become a design partner** | [Email me →](mailto:zhanghongping1982@gmail.com?subject=EcoCompute%20Design%20Partner) |
| 💼 **Invest / Grant** | [Email me →](mailto:zhanghongping1982@gmail.com?subject=EcoCompute%20Investment%20Inquiry) |

---

## 📚 Key Publications & Resources

- **Research Paper**: "When Does Quantization Save Energy? Empirical Analysis of the Energy-Efficiency Crossover Effect Across GPU Generations"
- **Dataset**: [GitHub](https://github.com/hongping-zh/ecocompute-ai) | [Zenodo DOI](https://zenodo.org/records/19647290)
- **HuggingFace Docs**: [Optimum Energy Efficiency Guide](https://huggingface.co/docs/optimum/)
- **MLCommons Discussion**: [Issue #2558](https://github.com/mlcommons/inference/issues/2558)

---

<p align="center">
  <i>🌍 Making AI development more sustainable, one model at a time.</i>
</p>
