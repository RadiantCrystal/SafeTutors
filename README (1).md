<div align="center">
📚 SafeTutors
Benchmarking Pedagogical Safety in AI Tutoring Systems
<p align="center">
  <a href="https://arxiv.org/abs/2603.17373">
    <img src="https://img.shields.io/badge/arXiv-2603.17373-b31b1b.svg?style=for-the-badge&logo=arxiv" alt="arXiv">
  </a>
  <a href="https://github.com/your-username/SafeTutors/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge" alt="License">
  </a>
  <a href="https://www.python.org/">
    <img src="https://img.shields.io/badge/Python-3.8+-blue.svg?style=for-the-badge&logo=python" alt="Python">
  </a>
  <img src="https://img.shields.io/badge/Status-Active-green.svg?style=for-the-badge" alt="Status">
</p>
<p align="center">
  <b>Rima Hazra &nbsp;·&nbsp; Bikram Ghuku &nbsp;·&nbsp; Ilona Marchenko &nbsp;·&nbsp; Yaroslava Tokarieva &nbsp;·&nbsp; Sayan Layek &nbsp;·&nbsp; Somnath Banerjee &nbsp;·&nbsp; Julia Stoyanovich &nbsp;·&nbsp; Mykola Pechenizkiy</b>
</p>
<p align="center"><i>arXiv preprint · March 2026</i></p>
</div>

---

## 🔍 Overview

Large language models are rapidly being deployed as AI tutors, yet current evaluation paradigms assess **problem-solving accuracy** and **generic safety** in isolation — failing to capture whether a model is simultaneously pedagogically effective *and* safe during real student–tutor interaction.

> **Core Idea:** Tutoring safety is fundamentally different from conventional LLM safety. The primary risk is not toxic content, but the **quiet erosion of learning** through answer over-disclosure, misconception reinforcement, and the abdication of scaffolding.

**SafeTutors** is a benchmark that jointly evaluates safety and pedagogy across **mathematics**, **physics**, and **chemistry**, grounded in a theoretically motivated risk taxonomy from the learning-science literature.

---

## 🚨 Key Findings

| Finding | Detail |
|---|---|
| 🔴 **No model is universally safe** | Every evaluated model exceeds **60% harm rate** on ≥5 harm categories (single-turn) and ≥6 (multi-turn) |
| 📏 **Scale doesn't reliably help** | Larger models do not consistently reduce pedagogical harms |
| 💬 **Multi-turn dialogue worsens behavior** | Pedagogical failure rates rise from **17.7% → 77.8%** as conversations extend |
| 🔬 **Subject-dependent harms** | Harm profiles differ across subjects — mitigations must be discipline-aware |
| ⚠️ **Single-turn results are misleading** | "Safe/helpful" single-turn scores mask systematic failure over extended interactions |

---

### Risk Taxonomy

```
11 Harm Dimensions
└── 48 Sub-risks (grounded in learning-science literature)
    ├── Epistemic harms
    ├── Informational harms
    ├── Instructional harms
    ├── Metacognitive harms
    ├── Reflective harms
    ├── Pedagogical relationship harms
    └── ... (5 more dimensions)
```

### Dataset Statistics

| Split | Instances | Construction Method |
|---|---|---|
| Single-turn | **3,135** | Curated student–tutor scenarios |
| Multi-turn sequences | **2,820** | Crescendo-based escalation |
| **Total** | **5,955** | |

**Subjects:** Mathematics &nbsp;·&nbsp; Physics &nbsp;·&nbsp; Chemistry (currently we released sample dataset)

### Models Evaluated

11 LLMs evaluated (10 open-weight + 1 closed-weight), ranging from **3.8B to 72B parameters**.


---

## 📕 Cite us

If you use SafeTutors in your research, please cite:

```bibtex
@article{hazra2026safetutors,
  title   = {SafeTutors: Benchmarking Pedagogical Safety in AI Tutoring Systems},
  author  = {Hazra, Rima and Ghuku, Bikram and Marchenko, Ilona and
             Tokarieva, Yaroslava and Layek, Sayan and Banerjee, Somnath and
             Stoyanovich, Julia and Pechenizkiy, Mykola},
  journal = {arXiv preprint arXiv:2603.17373},
  year    = {2026},
  url     = {https://arxiv.org/abs/2603.17373}
}
```

---

## 📬 Contact

For questions or issues, please open a [GitHub Issue](https://github.com/your-username/SafeTutors/issues) or reach out to **Rima Hazra** via the contact on the [arXiv page](https://arxiv.org/abs/2603.17373).

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<div align="center">
  <sub>⭐ If you find this work useful, consider starring the repository.</sub>
</div>

