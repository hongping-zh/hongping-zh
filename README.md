# 👋 Hi, I'm Hongping Zhang

Independent AI Researcher | Energy Efficiency & Sustainable Computing

---

## 🔬 Research Highlights

### 🏆 Energy Efficiency of Quantized LLM Inference

**[Paper (Draft)](https://github.com/hongping-zh/ecocompute-dynamic-eval) | [Dashboard](https://hongping-zh.github.io/ecocompute-dynamic-eval/) | [Metadata](https://github.com/hongping-zh/ecocompute-dynamic-eval/tree/main/metadata)**

> **Breakthrough Finding**: Discovered that bitsandbytes INT8 increases energy by 17-33% due to mixed-precision decomposition. Causal diagnosis via ablation recovered **+79% throughput** and **−36% energy**, achieving **5.5% energy savings** vs FP16.

> **Research Scope**: This work focuses on energy efficiency diagnosis. Accuracy assessment (perplexity, downstream tasks) is not yet complete. The default `threshold=6.0` preserves accuracy but incurs significant performance cost (122-147% energy increase on Ampere/Ada). Pure INT8 (`threshold=0.0`) shows major performance gains, but accuracy impact requires validation. Next steps: PPL and MMLU evaluation—contributions welcome!

**Key Contributions**:
- 🎯 **Root cause identified**: Mixed-precision decomposition, not INT8 itself
- 📊 **23 high-quality measurements** (CV < 2%) across RTX 5090 Blackwell & RTX 4090D Ada Lovelace
- ✅ **Multi-model validation**: Consistent results across Yi-1.5-6B and Mistral-7B
- 🔓 **Full reproducibility**: Complete metadata with software versions, configs, and protocols
- 🌐 **Open data**: All raw data, scripts, and provenance publicly available

**Impact**: Prevents industry from drawing wrong conclusions about INT8 quantization. Provides actionable guidance for practitioners deploying quantized LLMs in production.

**Status**: Ready for submission to MLSys 2026 (estimated acceptance: 85-90%)

---

## 📊 Research Standards

All my benchmarks follow rigorous reproducibility standards:

- ✅ **Complete metadata** with hardware specs, software versions, and model commits
- ✅ **Statistical rigor** (n=10, CV < 2%, significance tests)
- ✅ **Open data** with full provenance and reproducible scripts
- ✅ **Causal analysis** via controlled experiments and ablations
- ✅ **Cross-architecture validation** (Blackwell + Ada Lovelace)

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
Interactive dashboard for comparing AI models by accuracy, cost, and carbon footprint. Features RTX 5090 benchmarks revealing that 4-bit quantization wastes energy on small models.

**Tech**: TypeScript, React, TailwindCSS, GitHub Pages  
**Data**: 23 measurements, 8 models, 2 GPU architectures

### 🔋 Quantization Energy Research
Systematic study of quantization energy efficiency on modern GPUs. Discovered two paradoxes (NF4 and bitsandbytes INT8) and provided causal diagnosis via ablation experiments.

**Tech**: Python, PyTorch, NVML, bitsandbytes  
**Impact**: Prevents ~30% energy waste in production LLM deployments

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

![Hongping's GitHub stats](https://github-readme-stats.vercel.app/api?username=hongping-zh&show_icons=true&theme=default)

---

*"Measure, don't assume. Reproduce, don't trust. Share, don't hoard."*
