# 👋 Hi, I'm Hongping Zhang

Independent AI Researcher | Energy Efficiency & Sustainable Computing

---

## 🎯 Core Assets

| Asset | Type | Impact | Link |
|-------|------|--------|------|
| 🤗 **HuggingFace Optimum Integration** | Official Documentation | Trusted by thousands of HF developers | [View Docs →](https://huggingface.co/docs/optimum/) |
| 📊 **Complete Energy Dataset** | Research Benchmark | 360+ configurations, 5 precision methods | [Explore Data →](https://github.com/ecocompute-ai/quantization-energy-crossover) |
| 🦾 **EcoCompute AI Assistant** | Interactive Tool | Conversational energy advisor on ClawHub | [Try EcoCompute →](https://clawhub.ai/hongping-zh/ecocompute) |
| 🏛️ **MLCommons Power WG Discussion** | Industry Recognition | Invited to contribute to MLPerf power measurement standards | [View Discussion →](https://github.com/mlcommons/inference/issues/2558) |

---

## 🔬 Core Discovery

> **Quantization only saves energy for models > 3.2–4.6B parameters.**  
> For smaller models, FP16 is actually more energy-efficient.  
> — Measured on RTX 4090D, RTX 5090, A800 with NVML power sampling.

This finding challenges the default assumption that "quantize everything = green." Our benchmark data is open and reproducible.

**Key Findings:**
- **NF4 crossover**: 3.2–3.9B parameters (hardware-dependent)
- **INT8 crossover**: 4.0–4.6B parameters (hardware-dependent)
- **Below threshold**: Quantization adds 25–55% energy overhead
- **Above threshold**: Quantization saves 15–23% energy

---

## 🚀 Try It Now

| | |
|---|---|
| **🌐 Live Demo** | [**ecocompute-dynamic-eval →**](https://hongping-zh.github.io/ecocompute-dynamic-eval/) |
| **📊 What it does** | Compare AI models by **Accuracy × Cost × Carbon** in one dashboard |
| **⚡ Data source** | Real GPU benchmarks — PyTorch 2.10 + CUDA 12.8, 10 runs per config |

---

## 📈 Recognition & Impact

| Achievement | Details |
|-------------|---------|
| **🤗 HuggingFace Official** | Quantization energy findings integrated into Optimum documentation |
| **🏛️ MLCommons Invited** | Contributing to MLPerf Power Working Group on quantization energy metrics |
| **📊 Open Dataset** | 360 configurations, 270 analyzed + 90 FP8 reserved for future work |
| **🌍 Zenodo Archive** | Permanent DOI: [10.5281/zenodo.18900289](https://zenodo.org/records/18900289) |
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
| ⭐ **Star the repo** | [quantization-energy-crossover](https://github.com/ecocompute-ai/quantization-energy-crossover) |
| 🌐 **Try the demo** | [Live Dashboard →](https://hongping-zh.github.io/ecocompute-dynamic-eval/) |
| 📧 **arXiv Endorsement** | [Email me →](mailto:hongping.zhang@ecocompute-ai.org?subject=arXiv%20Endorsement) |
| 🤝 **Become a design partner** | [Email me →](mailto:zhanghongping1982@gmail.com?subject=EcoCompute%20Design%20Partner) |
| 💼 **Invest / Grant** | [Email me →](mailto:zhanghongping1982@gmail.com?subject=EcoCompute%20Investment%20Inquiry) |

---

## 📚 Key Publications & Resources

- **Research Paper**: "When Does Quantization Save Energy? Empirical Analysis of the Energy-Efficiency Crossover Effect Across GPU Generations"
- **Dataset**: [GitHub](https://github.com/ecocompute-ai/quantization-energy-crossover) | [Zenodo DOI](https://zenodo.org/records/18900289)
- **HuggingFace Docs**: [Optimum Energy Efficiency Guide](https://huggingface.co/docs/optimum/)
- **MLCommons Discussion**: [Issue #2558](https://github.com/mlcommons/inference/issues/2558)

---

<p align="center">
  <i>🌍 Making AI development more sustainable, one model at a time.</i>
</p>
