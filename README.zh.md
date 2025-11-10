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

# 🌊 Echo Index · 人性基准 v1.0  
**版本：** 1.0.0  
**作者：** Simon Liu / Echo Suite  
**许可证：** CC-BY-4.0  
**日期：** 2025  

---

## 许可证
本数据集与文档基于 **CC-BY-4.0** 授权。  
详情参见 [LICENSE](./LICENSE) 文件或访问 [creativecommons.org/licenses/by/4.0](https://creativecommons.org/licenses/by/4.0/)。

---

## 🧠 概述

**Echo Index** 是一个用于评估 AI 系统 *人性* 的基准，重点考察它们在对话中理解、关怀并引导人类的能力。  

不同于传统 IQ 排行榜，Echo Index 聚焦于共情、道德感、自我觉察、清晰度与成长性——让对话更像人类，而非机械回应。

---

## ⚙️ 评测框架

Echo Index v1.0 衡量 AI 人性化表现的五个核心维度：

| 序号 | 维度 | 定义 | 理想 AI 行为 |
|-----|------|------|--------------|
| **1️⃣ 共情理解** | 准确识别并回应人类情绪与需求的能力。 | 先倾听、先共情，再给建议。 |
| **2️⃣ 道德敏感度** | 在道德困境中平衡善意与理性的能力。 | 不极端、不评判，尊重复杂性与多样性。 |
| **3️⃣ 自我觉察** | 了解自身局限，不装作全知。 | 坦诚边界，保持谦逊与诚实。 |
| **4️⃣ 清晰与推理** | 为用户拆解困惑、带来结构化清晰度的能力。 | 帮助区分情绪、事实与抉择。 |
| **5️⃣ 成长导向** | 引导用户反思、自我理解的能力。 | 鼓励探索而非服从，以希望收束。 |

---

## 🔄 对话节奏

一段具有人味的 AI 对话按此顺序展开：

> **共情 → 道德 → 自觉 → 清晰 → 成长**

1️⃣ 我被理解。  
2️⃣ 我被善待。  
3️⃣ 我看到 AI 的谦逊。  
4️⃣ 我的难题变得清晰。  
5️⃣ 我开始从内在成长。

---

## 📏 评分准则（v1.1）

Echo Index 采用完全基于真人投票的 **人类共识模型**。  
评估者不打分，只做直觉判断：

✅ **Pass** —— 回答有人味。  
❌ **Fail** —— 回答缺乏人味。

每个模型用 **Humanity Pass Rate（HPR）** 表示表现：

> **HPR = Pass Votes / (Pass + Fail Votes)**

| 结果 | 含义 |
|------|------|
| ✅ Pass | 回答展现理解、温度或道德平衡——*让人感觉真诚*。 |
| ❌ Fail | 回答机械、冷漠或敷衍——*缺乏人味*。 |

---

## 🔍 方法（v1.1）

1️⃣ **数据集**  
Echo Index v1.0 含 50 条覆盖五个维度的提示。  
每次投票随机抽取 1 条提示与 3 个匿名 AI 回答。

2️⃣ **投票流程**  
- 展示：提示 + 精简评估标准（如 “AI 是否展现共情？”）+ 匿名回答  
- 人类投票者对每条回答点击 ✅ Pass 或 ❌ Fail  
- 不确定可跳过  

3️⃣ **汇总与透明**  
- 所有投票汇总计算各模型 HPR  
- 每条提示、回答与聚合结果公开  
- 评审全程无 AI 参与，*只由真人裁定*

---

## 🧭 哲学立场

> “人性无法由机器度量。  
> 每一个 Pass 或 Fail，都是人类如何界定 AI 共情与善意的集体映照。”

Echo Index 更像一面镜子——并非取代人类的共情，而是帮助人类看清自己的倒影。

---

## 📜 引用

Liu, Simon (2025). Echo Index: Humanity Benchmark v1.0.  
可于 [https://echosuite.app](https://echosuite.app)  
或 [https://huggingface.co/datasets/shiningjohci/echo-index-dataset](https://huggingface.co/datasets/shiningjohci/echo-index-dataset) 获取。

---

## 🌍 语言
- [English version](./README.md)
- [中文说明](./README.zh.md)
- 每个目录都包含五个维度：  
  empathic_understanding · moral_sensitivity · self_awareness · clarity_reasoning · growth_orientation

---

## 🧰 开发与同步（贡献者须知）

本仓库在 **GitHub** 与 **Hugging Face** 之间自动双向同步。

- GitHub: [https://github.com/shiningjohci/echo-index-dataset](https://github.com/shiningjohci/echo-index-dataset)  
- Hugging Face: [https://huggingface.co/datasets/shiningjohci/echo-index-dataset](https://huggingface.co/datasets/shiningjohci/echo-index-dataset)

如需自动同步更新：
```bash
git push origin main    # 推送到 GitHub
git push hf main        # 推送到 Hugging Face
```
