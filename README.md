# Vision-Language-Action Models

<div align="center">
  
  [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
  [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
  [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/username/vla-wiki/graphs/commit-activity)
  [![GitHub](https://img.shields.io/github/license/username/vla-wiki)](LICENSE)
  
  <h3>A curated wiki for researchers working at the intersection of Vision, Language, and Action in robotics</h3>
  
  [Getting Started](#getting-started) •
  [Papers](#papers) •
  [Models](#models) •
  [Datasets](#datasets) •
  [Tools](#tools) •
  [Contributing](#contributing)
  
  <img src="assets/vla-overview.png" alt="VLA Overview" width="600">
  
  *Bridging perception, language understanding, and robotic control*
  
</div>

---

## 📋 About

**Vision-Language-Action (VLA)** models represent a paradigm shift in robotics — unifying visual perception, natural language understanding, and motor control into end-to-end learned policies. This repository serves as a **living wiki** for the rapidly growing VLA research community.

Whether you're a PhD student just starting out, an industry researcher, or a curious engineer, this resource aims to help you navigate the landscape of models, datasets, benchmarks, and implementation tools in this exciting field.

### 🎯 Why this wiki?

- **Fragmented landscape** — VLA research spans robotics, CV, NLP, and RL
- **Fast-moving field** — New papers, models, and benchmarks emerge weekly
- **High entry barrier** — Need to navigate perception, reasoning, and control simultaneously

Our goal: **curate, organize, and make accessible** the collective knowledge of the VLA community.

---

## 🚀 Getting Started

New to VLA models? Start here:

| Resource | Description |
|---------|-------------|
| [📖 Background & Key Concepts](docs/background.md) | What are VLAs? Core architectures, training paradigms |
| [🎓 Tutorials & Courses](docs/tutorials.md) | Video lectures, blog posts, interactive notebooks |
| [📊 Evaluation Metrics](docs/evaluation.md) | How to evaluate VLA models |
| [⚙️ Setup Guide](docs/setup.md) | Environment setup, hardware recommendations |

---

## 📚 Papers

### 📑 Survey & Review Papers
| Year | Title | Venue | Links | TL;DR |
|------|-------|-------|-------|-------|
| 2024 | [Vision-Language-Action Models: A Survey](https://arxiv.org/abs/xxxx.xxxxx) | arXiv | [PDF]() | Comprehensive overview of the field |
| 2023 | [Foundation Models in Robotics](https://arxiv.org/abs/2312.07843) | arXiv | [PDF]() | Broader foundation models context |

### 🏛️ Foundational Works
| Year | Title | Venue | Links | Key Contribution |
|------|-------|-------|-------|------------------|
| 2023 | [RT-2: Vision-Language-Action Models](https://robotics-transformer2.github.io/) | RSS | [Paper](), [Code](), [Project]() | First large-scale VLA model |
| 2023 | [PaLM-E: An Embodied Multimodal Language Model](https://palm-e.github.io/) | ICLR | [Paper](), [Project]() | Embodied reasoning with LLMs |
| 2023 | [RoboFlamingo](https://roboflamingo.github.io/) | arXiv | [Paper](), [Code]() | Open-source VLA framework |
| 2022 | [SayCan: Do As I Can, Not As I Say](https://saycan.github.io/) | CoRL | [Paper](), [Project]() | Grounding LLMs in affordances |

### 🔬 Recent Advances (2024-2025)
| Title | Affiliation | Links | Highlights |
|-------|------------|-------|------------|
| [OpenVLA: An Open-Source Vision-Language-Action Model](https://openvla.github.io/) | Stanford/UC Berkeley | [Paper](), [Code]() | Fully open-source, LLaMA-based |
| [RoboMamba](https://robomamba.github.io/) | UCLA/CMU | [Paper](), [Code]() | Efficient Mamba-based VLA |
| [π0 (Pi-Zero)](https://physicalintelligence.company/) | Physical Intelligence | [Paper]() | Flow matching for robotic control |

<details>
<summary>📂 Browse by Category (Click to expand)</summary>

<br>

- **End-to-end VLAs** - RT-2, OpenVLA, RoboFlamingo
- **LLM/VLM-based Planners** - PaLM-E, SayCan, Code as Policies
- **Diffusion Policies** - Diffusion Policy, SuSIE
- **Hierarchical Approaches** - RT-H, LLM+P
- **Efficient VLAs** - RoboMamba, TinyVLA

[View full categorized list →](papers/README.md)

</details>

---

## 🤖 Models

### Pre-trained VLA Models
| Model | Release Date | Size | Base Model | Pretraining Data | Fine-tuning | License | Links |
|-------|--------------|------|------------|------------------|-------------|---------|-------|
| **OpenVLA-7B** | Mar 2024 | 7B | LLaMA-2 | Open X-Embodiment | LoRA | CC-BY-NC | [🤗](), [🐙]() |
| **RT-2-XL** | Dec 2023 | 55B | PaLI-X | WebLI + Robotics | Full | Proprietary | [🌐]() |
| **RoboFlamingo** | Oct 2023 | 3B | OpenFlamingo | Open X-Embodiment | LoRA | MIT | [🤗](), [🐙]() |
| **RoboMamba** | Jan 2024 | 1.8B | Mamba | RoboSet | Full | Apache-2.0 | [🤗](), [🐙]() |

### Model Components
- **Vision Encoders**: CLIP, SigLIP, DINOv2, ViT
- **Language Models**: LLaMA, Mistral, Phi, Mamba
- **Action Heads**: Diffusion, MLP, Transformer, Flow Matching

[Detailed model cards & comparisons →](models/README.md)

---

## 🗂️ Datasets & Benchmarks

### 🎯 Robotics Datasets
| Dataset | Year | Size | Tasks | Embodiments | Links |
|---------|------|------|-------|-------------|-------|
| **Open X-Embodiment** | 2023 | 1M+ episodes | Multi-task | 22 robots | [🌐]() |
| **BridgeData V2** | 2023 | 60k trajs | Manipulation | WidowX | [🌐]() |
| **DROID** | 2024 | 350k trajs | Manipulation | Franka | [🌐]() |
| **RLBench** | 2022 | 100 tasks | Simulated | Franka | [🌐]() |
| **CALVIN** | 2022 | 2.3M trajs | Long-horizon | Franka | [🌐]() |

### 📊 Benchmarks
| Benchmark | Domain | Metrics | SOTA Model | Links |
|-----------|--------|---------|------------|-------|
| **VLA-Bench** | 160 tasks across 10 envs | Success Rate, Efficiency | OpenVLA (78%) | [🌐]() |
| **RoboVQA** | Visual Question Answering | Accuracy | PaLM-E (84%) | [🌐]() |
| **SIMPLER** | Sim-to-real evaluation | Correlation | RT-2 (0.89) | [🌐]() |

[Complete dataset catalog →](datasets/README.md)

---

## 🛠️ Tools & Frameworks

### Training & Deployment
| Tool | Description | Language | Stars | Links |
|------|-------------|----------|-------|-------|
| **OpenVLA** | Open-source VLA training/fine-tuning | Python | 2.3k | [🐙]() |
| **RoboFlamingo** | Fine-tuning framework | Python | 1.1k | [🐙]() |
| **Octo** | Transformer-based policy | Python | 850 | [🐙]() |
| **LERF-TOGO** | Language-guided 3D reasoning | Python | 420 | [🐙]() |

### Simulation Environments
| Environment | Features | Robots | Links |
|-------------|----------|--------|-------|
| **Isaac Sim** | Photorealistic, GPU-accelerated | Franka, UR, custom | [🌐]() |
| **RoboSuite** | Modular, gym-compatible | WidowX, Franka | [🐙]() |
| **PyBullet** | Lightweight, fast | Many | [🌐]() |
| **Habitat** | Navigation, rearrangement | Fetch, Stretch | [🐙]() |

[Comprehensive tools list →](tools/README.md)

---

## 🧪 Evaluation & Reproducibility

- [**VLA Evaluation Suite**](https://github.com/example/vla-eval) — Standardized evaluation protocol
- [**Checklist for Reproducibility**](docs/reproducibility.md) — Ensure your work is reproducible
- [**Common Pitfalls**](docs/pitfalls.md) — Learn from others' mistakes

---

## 📈 Research Trends & Analysis

- **2023**: Emergence of large-scale VLAs (RT-2, PaLM-E)
- **2024**: Shift toward open-source, efficient models (OpenVLA, RoboMamba)
- **2025**: Multi-robot generalization, sim2real, compositional VLAs

[Quarterly field analysis →](trends/README.md)

---

## 👥 Community & Contributing

This is a community-maintained repository. We warmly welcome contributions!

### How to Contribute
1. **Add a paper/model/tool**: Submit a PR with the addition
2. **Suggest improvements**: Open an issue
3. **Review submissions**: Help maintain quality

Please see our [contribution guidelines](CONTRIBUTING.md) and [code of conduct](CODE_OF_CONDUCT.md).

### Contributors
<a href="https://github.com/username/vla-wiki/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=username/vla-wiki" />
</a>

Made with [contrib.rocks](https://contrib.rocks).

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details. The content is freely available for adaptation and reuse with attribution.

---

## 📬 Contact & Citation

If you find this wiki useful for your research, please consider citing it:

```bibtex
@misc{vlawiki2025,
  author = {VLA Community},
  title = {Vision-Language-Action Models Wiki},
  year = {2025},
  publisher = {GitHub},
  journal = {GitHub Repository},
  howpublished = {\url{https://github.com/ishandutta2007/vla-wiki}}
}
```

**Maintainers**: [@ishandutta2007](https://github.com/ishandutta2007)

---

<div align="center">
  <sub>⭐ Star this repo if you find it useful — it helps others discover it!</sub>
  <br>
  <sub>Last updated: February 2025</sub>
</div>

## ✨ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=ishandutta2007/Vision-Language-Action&type=date&legend=top-left)](https://www.star-history.com/#ishandutta2007/Vision-Language-Action&type=date&legend=top-left)
