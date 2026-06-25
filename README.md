# PaperReading

linzy 的个人论文阅读笔记项目，围绕**高能物理 · 量子色动力学（QCD）**展开，核心研究方向是**胶球（glueball）**——一种由胶子自相互作用形成的、QCD 非阿贝尔结构预言的奇异强子。

## 项目简介

这个仓库用 LaTeX 整理我读过的论文，按主题分章节，每篇论文一条中文笔记，配合 BibTeX 引用。目标是把分散的文献组织成可检索、可回顾的知识库，方便日后写综述、毕业论文或研究汇报时调用。

笔记里有两类内容：
- 对论文方法、关键结果的中文总结
- 用红色 `\textcolor{red}{...}` 标注的**重点**——方法学关键点、值得深入研究的方向、或自己尚未完全想清楚的问题

## 章节结构

### Glueball 核心
| 章节 | 内容 |
|------|------|
| Glueball (different method and else) | 不同方法（势模型、光前、全息、BSE、格点等）对胶球的计算 |
| Glueball (mass spectrum) | 胶球质量谱的相关工作 |
| Glueball (review) | 综述类文献 |
| Glueball (color and Cparity) | 胶球的颜色空间结构和 C 宇称分析 |
| Glueball (experiment) | 实验上寻找胶球的努力（BESIII 等） |
| Glueball (Candidate) | 胶球候选态的实验和理论分析（$f_0(1500)$、$f_0(1710)$、$X(2370)$ 等） |
| Decay | 胶球及相关的衰变过程 |

### 方法论与相关主题
| 章节 | 内容 |
|------|------|
| QCD Theory | QCD 基础理论（色因子、对称性等） |
| Structure Function | 部分子分布函数（PDF）、TMD、GPD 等 |
| GFF | 引力形状因子（Gravitational Form Factors） |
| Review | 综述与方法学介绍 |
| DEMELO Suggestion | de Melo 系列关于光前协变性、零模、形状因子的工作 |
| blfq method | 基光前量子化（Basis Light-Front Quantization, BLFQ）方法 |
| AI4Science | 神经网络 / 机器学习在强子物理中的应用 |

## 工具链

- **排版**：`pdflatex` + `bibtex`，使用 `ctex` 中文支持
- **引用**：`sample.bib`（BibTeX 格式，扁平管理）
- **构建**：
  ```bash
  pdflatex main.tex
  bibtex main
  pdflatex main.tex
  pdflatex main.tex
  ```

## 笔记风格示例

```latex
\subsection{论文标题}

Title: \quad 论文标题 \cite{bibkey}

中文笔记内容，介绍方法、关键结果、与自己研究的关联。
重点内容用 \textcolor{red}{...} 标红。
```

## 联系

研究者：**linzy@impcas.ac.cn**  
研究方向：胶球（glueball）物理 / 量子色动力学 / AI4Science / 矩阵微扰理论
