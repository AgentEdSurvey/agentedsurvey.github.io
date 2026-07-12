# 🤖 Multi-Agent LLM Systems for Psychology, Behavior, and Education

## 🧠 面向心理学、行为与教育的多智能体 LLM 系统：系统综述

<p align="center">
  <a href="./paper/manuscript.pdf">
    <img src="https://img.shields.io/badge/Paper-Under%20Review-3b82f6?style=for-the-badge&logo=readthedocs&logoColor=white" alt="Paper"/>
  </a>
  <a href="./data/full_corpus_101.csv">
    <img src="https://img.shields.io/badge/Corpus-101%20Studies-16a34a?style=for-the-badge&logo=databricks&logoColor=white" alt="Corpus"/>
  </a>
  <a href="./data/coding_matrix_full.csv">
    <img src="https://img.shields.io/badge/Coding-Full%20Matrix-f97316?style=for-the-badge&logo=tableau&logoColor=white" alt="Coding Matrix"/>
  </a>
  <a href="https://AgentEdSurvey.github.io/">
    <img src="https://img.shields.io/badge/Project-Website-8b5cf6?style=for-the-badge&logo=githubpages&logoColor=white" alt="Project Website"/>
  </a>
</p>

> 📘 This repository accompanies the manuscript  
> **“Multi-Agent LLM Systems for Psychology, Behavior, and Education: A Systematic Survey.”**

> 📚 本仓库提供该系统综述的检索记录、101 篇研究语料、编码矩阵、统计结果、编码手册与补充材料。

---

## 🌐 Overview / 项目简介

Psychology, behavior, and education are interaction-rich domains in which constructs such as cognitive distortion, trust, conformity, theory of mind, misconceptions, and higher-order thinking are rarely observable as isolated labels.

This survey examines how multi-agent LLM systems translate latent psychological, behavioral, and educational constructs into inspectable interaction processes through role assignment, orchestration, grounding, memory, critique, consensus, and human validation.

心理学、行为学与教育学中的许多核心构念并非孤立标签，而是在交互、记忆、反馈与社会情境中逐步显现。本综述关注多智能体 LLM 系统如何通过角色分工、工作流编排、知识与记忆、批判反思、共识形成和人工验证，将这些潜在构念转化为可检查的交互过程。

📌 **Current corpus:** 101 studies  
📌 **Coding logic:** non-exclusive multi-label dimensions  
📌 **Main focus:** psychology, behavior, education, and human-agent collaboration

---

## ✨ Key Contributions / 主要贡献

### 📚 1. Systematic Corpus

A structured corpus of **101 studies** spanning NLP, HCI, psychology, education, computational social science, and health-related research.

### 🧭 2. Four Application Domains

- 🧠 Psychological assessment and mental health
- 🎭 Behavioral and social simulation
- 📖 Education, learning, and assessment
- 🤝 Human-agent collaboration and cognitive modeling

### 🏗️ 3. Five Non-Exclusive Architectural Mechanisms

- 🔗 Functional pipeline
- 💬 Deliberative debate
- 👥 Persona-based social simulation
- 🎮 Game or self-play
- 📚 Grounded workflow

### 🔄 4. Five-Stage Process Framework

**Theory Mapping → Orchestration → Grounding and Memory → Critique Loop → Validation**

### ✅ 5. Evaluation and Reporting Framework

- 🎯 Construct validity
- 🔁 Reliability
- 🧍 Behavioral realism
- 🎓 Pedagogical impact
- 🛡️ Safety and fairness
- 👩‍🏫 Human validation

---

## 🗂️ Repository Structure / 仓库结构

```text
.
├── 📄 README.md
├── ⚖️ LICENSE
├── 🧾 CITATION.cff
│
├── 📁 data/
│   ├── full_corpus_101.csv
│   ├── full_corpus.bib
│   ├── coding_matrix_full.csv
│   ├── corpus_statistics.csv
│   ├── selection_audit.csv
│   ├── coding_manual.md
│   └── DATA_README.md
│
├── 🔍 search/
│   ├── 1-500.ris
│   ├── 501-2805.ris
│   ├── conference_candidates.xlsx
│   ├── engineering_village_500.csv
│   ├── rayyan_candidates.csv
│   └── screening_decisions_anonymized.csv
│
├── 🖼️ figures/
│   ├── figure1.png
│   ├── figure2.png
│   ├── figure3.png
│   └── figure4.png
│
└── 🌐 index.html
```

---

## 📦 Data Files / 数据文件

### 📘 Full Corpus

- 📄 [Full 101-study corpus](./data/full_corpus_101.csv)
- 📚 [Full BibTeX bibliography](./data/full_corpus.bib)

`full_corpus_101.csv` contains:

- 🆔 study ID
- 📝 title
- 👤 authors
- 📅 year
- 🏛️ venue
- 🗃️ publication type
- 🔗 DOI or official URL
- 📂 source file
- ✅ selection basis
- 🔎 reconstruction status
- ℹ️ metadata status

### 🧩 Coding Matrix

- 📊 [Full coding matrix](./data/coding_matrix_full.csv)
- 📕 [Coding manual](./data/coding_manual.md)

The coding matrix records:

- 🧠 application domains
- 🏗️ architectural mechanisms
- ⚙️ process components
- 🎯 evaluation targets
- 👩‍🏫 human-validation status

### 📈 Corpus Statistics

- 📉 [Corpus statistics](./data/corpus_statistics.csv)

This file summarizes publication years, publication types, and conservative coding counts.

### 🔍 Selection Audit

- 🧾 [Selection and matching audit](./data/selection_audit.csv)

This file documents how each record was retained, matched, and sourced.

### 📑 Data Documentation

- 📘 [Data README](./data/DATA_README.md)

This file explains the status, scope, and limitations of the reconstructed corpus package.

---

## 🔎 Search Records / 检索记录

The [`search/`](./search/) directory contains raw and intermediate search records, including:

- 📄 RIS exports
- 🗃️ Engineering Village results
- 🎓 conference candidate records
- 🧪 Rayyan candidate records
- 🔐 anonymized screening decisions

These files document the retrieval and screening process but should **not** be interpreted as the final included corpus.

`search/` 目录保存原始及中间检索记录，用于展示候选文献如何进入筛选流程；这些文件不等同于最终纳入的 101 篇语料。

---

## 🧭 Coding Framework / 编码框架

### 🧠 Application Domains

| Code | Meaning |
|---|---|
| `Psy` | Psychological assessment and mental health |
| `Beh` | Behavioral and social simulation |
| `Edu` | Education, learning, and assessment |
| `H-A` | Human-agent collaboration and cognitive modeling |

### 🏗️ Architectural Mechanisms

These mechanisms are **non-exclusive**.

| Code | Meaning |
|---|---|
| `Pipe` | Functional pipeline |
| `Deb` | Deliberative or debate-based collaboration |
| `Soc` | Persona-based social simulation |
| `Game` | Game-theoretic or self-play mechanisms |
| `GrdW` | Grounded workflow |

### ⚙️ Process Components

| Code | Meaning |
|---|---|
| `Role` | Role or persona initialization |
| `Mem` | Memory or interaction history |
| `Grd` | External grounding |
| `Ref` | Critique, reflection, review, or adjudication |
| `Con` | Consensus, synthesis, voting, or conflict resolution |

### 🎯 Evaluation Targets

| Code | Meaning |
|---|---|
| `CV` | Construct validity |
| `Rel` | Reliability and robustness |
| `BR` | Behavioral realism |
| `Ped` | Pedagogical impact |
| `Safe` | Safety and fairness |

### 👩‍🏫 Human Validation

| Value | Meaning |
|---|---|
| `Yes` | Explicit human or expert validation |
| `Partial` | Limited or indirect human validation |
| `No` | No human validation reported |

---

## 🔄 Five-Stage Design Workflow / 五阶段设计流程

<p align="center">
  <img src="./figures/figure3.png" width="72%" alt="Five-stage design workflow"/>
</p>

### 1️⃣ Theory Mapping

Map psychological, behavioral, or educational constructs to agent roles and responsibilities.

### 2️⃣ Orchestration

Select an interaction mechanism such as pipeline coordination, debate, self-play, or graph-based collaboration.

### 3️⃣ Grounding and Memory

Integrate external evidence, knowledge graphs, rubrics, curricula, interaction histories, or learner profiles.

### 4️⃣ Critique Loop

Introduce reviewers, critics, judges, or adversarial agents to evaluate logic, factuality, bias, and safety.

### 5️⃣ Validation

Synthesize outputs, preserve uncertainty, compare with benchmarks, and route high-stakes decisions to human review.

---

## 📌 Corpus Status / 语料状态说明

The current 101-study package was reconstructed from:

1. 📖 studies explicitly cited in the submitted manuscript;
2. 🔍 eligible records selected from the supplied candidate exports.

The repository includes `selection_audit.csv` to make the source and matching status of every record transparent.

当前 101 篇语料由两部分构成：

1. 投稿论文中明确引用的研究；
2. 从作者提供的候选导出记录中筛选出的合适研究。

为保证透明度，仓库同时提供 `selection_audit.csv`，记录每条文献的来源、匹配方式与状态。

> ⚠️ **Important:** The coding matrix uses conservative title/abstract-level coding where full-text confirmation was unavailable. Blank cells mean “not safely inferable,” not necessarily “absent.”

> ⚠️ **重要说明：** 在无法完成全文确认的情况下，编码矩阵采用保守的标题/摘要层级编码。空白单元格表示“无法安全判断”，不一定表示该特征不存在。

---

## 📊 Corpus Statistics / 语料统计

### 📅 Publication Year

| Year | Studies |
|---|---:|
| 2023 | 5 |
| 2024 | 21 |
| 2025 | 57 |
| 2026 | 18 |

> 2026 is incomplete because the corpus was closed before the end of the year.

Architecture and evaluation counts should be generated from the latest verified coding matrix rather than entered manually.

---

## ♻️ Reproducibility / 可复现性

The repository is designed to support:

- 🔍 inspection of the final 101-study corpus
- 🧩 inspection of all coding labels
- 🔗 verification of publication metadata
- 📈 reconstruction of summary statistics
- 🧾 auditing of record selection and matching
- 📚 reuse of the complete BibTeX bibliography

Future releases may add:

- 📉 PRISMA flow counts
- ❌ full-text exclusion reasons
- 🤝 independent coding reliability statistics
- 🧮 scripts for regenerating figures and cross-tabulations

---

## ⚠️ Limitations / 局限性

- 🔎 The corpus is shaped by the selected databases, search terminology, and corpus cut-off date.
- 🧩 Related work using adjacent terms such as collaborative prompting, ensemble deliberation, or role-based prompting may be underrepresented.
- 📝 The corpus includes recent preprints where these were part of the review scope.
- 🌍 English-language databases and major NLP, AI, HCI, psychology, and education venues are overrepresented.
- 🧪 The reconstructed coding package should be interpreted as an auditable working release rather than a substitute for full-text double coding and formal inter-coder reliability analysis.

---

## 📖 Citation

During anonymous review, please cite the manuscript as:

```bibtex
@misc{anonymous2026multiagent,
  title = {Multi-Agent LLM Systems for Psychology, Behavior, and Education:
           A Systematic Survey},
  author = {Anonymous},
  year = {2026},
  note = {Manuscript under review}
}
```

The citation will be updated after publication.

---

## 🕵️ Anonymous Review Notice / 匿名评审说明

This repository is prepared for anonymous review.

Author names, institutional affiliations, personal email addresses, and identifying metadata should be removed from the public materials.

本仓库用于匿名评审。公开材料中不应包含作者姓名、机构、个人邮箱或其他可识别身份的信息。

---

## ⚖️ License

- 📊 Author-created annotations, coding documentation, figures, and summary tables: **CC BY 4.0**
- 💻 Code: **MIT License**
- 🔗 Third-party bibliographic metadata and linked publications: subject to their original licenses
- 🚫 Copyrighted article PDFs are not redistributed in this repository

---

## 📬 Contact

Contact information will be added after the anonymous review period.
