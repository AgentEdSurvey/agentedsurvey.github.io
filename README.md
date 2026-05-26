# Multi-Agent LLM Systems for Psychology, Behavior, and Education
# 面向心理学、行为与教育的多智能体LLM系统：系统综述

[![Paper](https://img.shields.io/badge/Paper-EMNLP%202026-blue)](你的论文链接)
[![Survey](https://img.shields.io/badge/Corpus-101%20Studies-green)](./data/)
[![License](https://img.shields.io/badge/License-CC--BY%204.0-lightgrey)](./LICENSE)

&gt; **系统综述**：我们分析了101项研究，提出四领域应用分类、五类架构家族与五阶段设计流程框架。

[中文摘要](#摘要) | [Key Contributions](#key-contributions) | [Taxonomy](#taxonomy) | [Citation](#citation)

---

## 🔍 摘要 / Abstract

心理学与教育学是交互密集型领域。本综述回顾了 **101项研究**（56篇期刊，45篇会议论文），系统梳理了多智能体LLM系统在**心理评估、行为模拟、教育支持、人机协作**四大领域的应用。

**核心洞见**：多智能体系统最有价值的时刻，是将潜在的心理学或教育学构念（constructs）转化为**可检视的交互过程**。

---

## ✨ Key Contributions

1. **Systematic Corpus**: 101 studies identified through systematic search across NLP, HCI, Education, and Psychology
2. **Four Application Domains**:
   - 🧠 Psychological & Mental-Health Assessment
   - 🎭 Behavioral & Social Simulation  
   - 📚 Education, Learning & Assessment
   - 🤝 Human-Agent Collaboration
3. **Five Architectural Families**:
   - Functional Pipeline | Deliberative Debate | Persona Society | Game/Self-play | Grounded Workflow
4. **Process-Level Framework**: Theory Mapping → Orchestration → Grounding & Memory → Critique Loop → Validation
5. **Evaluation Guidelines**: Construct validity, reliability, behavioral realism, pedagogical impact, safety

---

## 📊 Taxonomy Overview

| 维度 | 分类 |
|------|------|
| **应用领域** | Psy / Beh / Edu / H-A |
| **架构家族** | Pipe / Deb / Soc / Game / GrdW |
| **核心组件** | Role / Mem / Grd / Ref / Con |
| **评估目标** | CV / Rel / BR / Ped / Safe |

&gt; 完整编码矩阵见 [Appendix D](./data/coding_matrix.csv)（如提供）

---

## 🏗️ Five-Stage Design Workflow

![Design Workflow](./assets/figures/figure3_workflow.png)

1. **Theory Mapping**: 将构念映射到智能体角色
2. **Orchestration**: 选择协调机制（规划、辩论、自博弈）
3. **Grounding & Memory**: 附加证据、知识图谱、学习者画像
4. **Critique Loop**: 引入评审者检验逻辑与偏见
5. **Validation**: 综合共识并与基准比较，路由至人工审核

---

## 📈 Corpus Statistics

- **时间跨度**: 2023–2026 (2026 incomplete)
- **增长趋势**: 2023(5) → 2024(21) → 2025(57) → 2026(18)
- **主导领域**: Education (59.4%), Grounded Workflow (48.5%)
- **评估重点**: Human Validation (56.4%), Pedagogical Impact (43.6%)

---

## ⚠️ Open Challenges

- **Validity Beyond Plausibility**: 合理性不等于有效性
- **Agent Diversity**: 同模型同提示的"多智能体"可能产生相关错误
- **Prompt Sensitivity**: 提示词的微小变化可能改变人格行为
- **Oversight in High-Stakes**: 心理健康与教育评估需要人类监督
- **Transparent Reporting**: 建议公开提示词、模型版本、解码参数

---

## 📖 Citation

如果你使用了本综述的分类框架或编码矩阵，请引用：

```bibtex
@inproceedings{anonymous2026survey,
  title={Multi-Agent LLM Systems for Psychology, Behavior, and Education: A Systematic Survey},
  booktitle={Proceedings of EMNLP 2026},
  year={2026}
}
