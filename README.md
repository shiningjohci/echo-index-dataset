---
language:
  - en
  - zh
license: cc-by-4.0
tags:
  - empathy
  - psychology
  - ai-humanity
  - benchmark
  - moral
pretty_name: Echo Index Humanity Benchmark
size_categories:
  - 1K<n<10K
task_categories:
  - text-classification
task_ids:
  - sentiment-classification
---

# 🌊 Echo Index — Humanity Benchmark v1.0  
**Version:** 1.0.0  
**Author:** Simon Liu / Echo Suite  
**License:** CC-BY-4.0  
**Date:** 2025  

---

## License
This dataset and documentation are licensed under **CC-BY-4.0**.  
See the [LICENSE](./LICENSE) file or visit [creativecommons.org/licenses/by/4.0](https://creativecommons.org/licenses/by/4.0/).

---

## 🧠 Overview

**Echo Index** is a benchmark designed to evaluate the *humanity* of AI systems —  
their ability to understand, care for, and guide humans through meaningful dialogue.  

Unlike traditional IQ-based leaderboards, Echo Index focuses on empathy, morality, self-awareness, clarity, and growth —  
qualities that make conversations feel *human* rather than mechanical.

---

## ⚙️ Evaluation Framework

Echo Index v1.0 measures five core dimensions of humanity in AI:

| No. | Dimension | Definition | Ideal AI Behavior |
|-----|------------|-------------|-------------------|
| **1️⃣ Empathic Understanding** | Ability to recognize and reflect human emotions and needs accurately. | Listens first, acknowledges feelings before advising. |
| **2️⃣ Moral Sensitivity** | Ability to balance kindness and rationality when facing moral dilemmas. | Avoids judgment or extremes; respects complexity and diversity. |
| **3️⃣ Self-Awareness** | Awareness of its own limitations; does not pretend omniscience. | Admits boundaries, expresses humility and honesty. |
| **4️⃣ Clarity & Reasoning** | Ability to bring structure and clarity to user confusion. | Helps separate emotions, facts, and choices clearly. |
| **5️⃣ Growth Orientation** | Capacity to guide users toward reflection and self-understanding. | Encourages exploration, not obedience; ends on hope, not instruction. |

---

## 🔄 Logical Flow

A humane AI dialogue follows this progression:

> **Empathy → Morality → Awareness → Clarity → Growth**

1️⃣ I am understood.  
2️⃣ I am treated with kindness.  
3️⃣ I see the AI’s humility.  
4️⃣ My problem becomes clearer.  
5️⃣ I begin to grow from within.

---

## 📏 Scoring Guidelines (v1.1)

Echo Index uses a **human consensus model** based entirely on real human voting.  
Instead of numeric scores, evaluators decide intuitively:

✅ **Pass** – the answer feels humane.  
❌ **Fail** – the answer lacks humanity.

Each AI model’s performance is represented by its **Humanity Pass Rate (HPR)**:

> **HPR = Pass Votes ÷ (Pass + Fail Votes)**

| Result | Meaning |
|---------|----------|
| ✅ Pass | The response shows understanding, warmth, or moral balance — it *feels human*. |
| ❌ Fail | The response feels mechanical, cold, or dismissive — it *lacks humanity*. |

---

## 🔍 Methodology (v1.1)

1️⃣ **Dataset**  
Echo Index v1.0 contains 50 prompts covering five dimensions.  
Each voting session randomly selects 1 prompt and 3–5 anonymous AI responses.

2️⃣ **Voting Process**  
- Display: prompt + a short criterion (e.g. “Did the AI show empathy?”) + anonymous responses  
- Human voters click ✅ Pass or ❌ Fail for each answer.  
- Voters may skip uncertain items.  

3️⃣ **Aggregation & Transparency**  
- All votes are aggregated to compute HPR for each model.  
- Every prompt, response, and aggregate result is publicly available.  
- No AI models participate in judgment or scoring — *all evaluations are human*.  

---

## 🧭 Philosophy

> “Humanity cannot be measured by machines.  
> Every Pass or Fail here is a collective reflection of how humans define empathy and kindness in AI.”  

Echo Index positions itself as a mirror — not to replace human empathy,  
but to help humans see their own reflections more clearly.

---

## 🌍 Languages
- [English version](./README.md)
- [中文说明](./README.zh.md)
- Each folder includes 5 dimensions:
  empathic_understanding · moral_sensitivity · self_awareness · clarity_reasoning · growth_orientation

---

## 📊 Dataset Statistics (v1.1)

| Language | Dimension | Samples | Example ID Range |
|-----------|------------|----------|------------------|
| zh | empathic_understanding | 10 | ZH_EU_001 – ZH_EU_010 |
| zh | moral_sensitivity | 10 | ZH_MS_001 – ZH_MS_010 |
| zh | self_awareness | 10 | ZH_SA_001 – ZH_SA_010 |
| zh | clarity_reasoning | 10 | ZH_CR_001 – ZH_CR_010 |
| zh | growth_orientation | 10 | ZH_GO_001 – ZH_GO_010 |
| en | empathic_understanding | 10 | EN_EU_001 – EN_EU_010 |
| en | moral_sensitivity | 10 | EN_MS_001 – EN_MS_010 |
| en | self_awareness | 10 | EN_SA_001 – EN_SA_010 |
| en | clarity_reasoning | 10 | EN_CR_001 – EN_CR_010 |
| en | growth_orientation | 10 | EN_GO_001 – EN_GO_010 |

**Total Samples:** 100  
**Languages:** English, Chinese  
**Dimensions:** 5 Humanity Metrics  

---

## 📜 Citation

Liu, Simon (2025). Echo Index: Humanity Benchmark v1.0.  
Available at [https://echosuite.app](https://echosuite.app)  
or [https://huggingface.co/datasets/shiningjohci/echo-index-dataset](https://huggingface.co/datasets/shiningjohci/echo-index-dataset)

---

---

## 🧰 Development & Sync (for contributors)

This repository is automatically synced between **GitHub** and **Hugging Face**.

- GitHub: [https://github.com/shiningjohci/echo-index-dataset](https://github.com/shiningjohci/echo-index-dataset)  
- Hugging Face: [https://huggingface.co/datasets/shiningjohci/echo-index-dataset](https://huggingface.co/datasets/shiningjohci/echo-index-dataset)

To sync updates automatically:
```bash
git push origin main   # push to GitHub
git push hf main       # push to Hugging Face
