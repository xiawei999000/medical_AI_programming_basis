
<div align="center">

# 📖 《医学AI编程基础：原理与实践》

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-red?logo=pytorch)](https://pytorch.org/)
[![Qwen Code](https://img.shields.io/badge/AI%20辅助-Qwen%20Code智能体-purple)](https://chat.qwen.ai/)

**上海交通大学医学院医学技术学院 教材配套开源代码仓库**


</div>

---

## 📌 简介

本仓库为上海交通大学医学院医学技术学院《AI编程基础》、《智能影像技术》课程教学资源与智能体的配套开源代码库，收录《医学AI编程基础：原理与实践》的 Jupyter Notebook 交互式实践代码（`.ipynb`）及所用医学数据集索引。

面向**医学相关专业研究生**，聚焦医学AI核心痛点，系统整合「**AI基础原理 — Python编程实现 — 医学场景应用**」三位一体。

> 📢 **本仓库所有代码均可一键运行**，无需额外配置，克隆仓库后按照环境说明安装依赖即可直接执行全书各章节 `.ipynb` 文件。

---

## 📚 教材结构与代码目录

```
medical-ai-programming/
│
├── Part1_Basics/               # 第一部分：基础篇（第 1—3 章）
│   ├── Ch01_MedicalAI_Overview/        # 第1章 医学AI概论
│   ├── Ch02_Dev_Environment/           # 第2章 医学AI编程开发环境搭建
│   └── Ch03_Python_Basics/             # 第3章 Python基础语法与医学AI编程实践
│
├── Part2_MachineLearning/      # 第二部分：机器学习篇（第 4—6 章）
│   ├── Ch04_Supervised_Learning/       # 第4章 有监督学习算法原理与医学数据分析实践
│   ├── Ch05_Unsupervised_Learning/     # 第5章 无监督学习算法原理与医学数据分析实践
│   └── Ch06_SemiSupervised_Learning/   # 第6章 半监督学习算法原理与医学数据分析实践
│
├── Part3_DeepLearning/         # 第三部分：深度学习篇（第 7—8 章）
│   ├── Ch07_ANN/                       # 第7章 人工神经网络原理与医学数据分析实践
│   └── Ch08_CNN/                       # 第8章 卷积神经网络原理与医学数据分析实践
│
├── Appendix/                   # 附录
│   ├── AppA_Python_Cheatsheet.md       # 附录A Python常用库速查
│   ├── AppB_Medical_Datasets.md        # 附录B 医学数据集资源
│   └── AppC_Repo_Links.md              # 附录C 数据集与代码仓库索引
│
├── requirements.txt            # 依赖库列表
├── environment.yml             # Conda 环境配置文件
└── README.md
```

---

## 🧭 各章内容概览

### 第一部分·基础篇（第 1—3 章）

| 章节 | 主要内容 | 配套代码 |
|------|----------|----------|
| 第1章 医学AI概论 | AI发展历程、机器学习与深度学习的层级关系、医学AI典型应用 | — |
| 第2章 开发环境搭建 | Python/Anaconda配置、核心AI库安装、PyCharm + Jupyter Notebook + **Qwen Code** 工具链配置 | — |
| 第3章 Python基础语法 | 数据类型、控制流程、NumPy/Pandas科学计算、医学数据可视化、代码规范 | `Ch03_python_basics.ipynb` |

### 第二部分·机器学习篇（第 4—6 章）

| 章节 | 主要内容 | 配套代码                                  |
|------|----------|---------------------------------------|
| 第4章 有监督学习 | 线性模型、KNN、决策树、随机森林、XGBoost、SVM、交叉验证、SHAP可解释性 | Ch04_supervised_learning.ipynb        |
| 第5章 无监督学习 | K-means、层次聚类、DBSCAN、PCA、t-SNE、UMAP、异常检测 | Ch05_unsupervised_learning.ipynb      |
| 第6章 半监督学习 ⭐ | 伪标签算法、自训练方法、标签传播算法、与有监督学习性能对比 | Ch06_semi-supervised_learning.ipynb |

> ⭐ 第6章"半监督学习"为本教材特色章节，专门应对医学场景「标注数据稀缺」的核心痛点，在同类教材中属首创。

### 第三部分·深度学习篇（第 7—8 章）

| 章节 | 主要内容 | 配套代码           |
|------|----------|----------------|
| 第7章 人工神经网络 | GPU/CUDA配置、张量与计算图、前向/反向传播、PyTorch全连接网络、批归一化、Dropout、早停 | Ch07_ANN.ipynb |
| 第8章 卷积神经网络 | 卷积/池化原理、LeNet/AlexNet/VGGNet/ResNet演进、医学图像分类、U-Net医学图像分割 | Ch08_CNN.ipynb |

---

## 🛠️ 开发环境

### 核心工具链（三位一体）

| 工具 | 版本 | 用途 |
|------|------|------|
| **PyCharm** | 2024.x+ | 专业Python IDE，工程开发、调试、Git管理 |
| **Jupyter Notebook** | 7.x+ | 交互式编程，全书代码以 `.ipynb` 格式配套 |
| **Qwen Code** | v0.10.5+ | 国产AI编程智能体，代码补全、中文解释、调试辅导 |

### 主要依赖库

```txt
Python >= 3.8
numpy
pandas
matplotlib
seaborn
scikit-learn
opencv-python
SimpleITK
torch >= 2.0
torchvision
jupyter
```

### 快速安装

**方法一：使用 Conda（推荐）**

```bash
git clone https://github.com/your-username/medical-ai-programming.git
cd medical-ai-programming
conda env create -f environment.yml
conda activate medical-ai
jupyter notebook
```

**方法二：使用 pip**

```bash
git clone https://github.com/your-username/medical-ai-programming.git
cd medical-ai-programming
pip install -r requirements.txt
jupyter notebook
```

> 💡 **国内用户加速建议**：安装前可配置清华镜像源以加速下载
> ```bash
> pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
> ```

---

## 🤖 Qwen Code 编程智能体配置

本教材配套使用 **Qwen Code**（通义千问编程智能体）作为 AI 辅助学习工具，原生支持中文，无需特殊网络配置，适合国内高校使用。

**在 PyCharm 中安装（详见教材第 2.3.3 节）：**

1. 打开 `File → Settings → Tools → AI Assistant → 代理`
2. 搜索 `Qwen Code`，选择 **Alibaba Qwen Team** 发布的版本，点击安装
3. 在 PyCharm 终端中输入 `qwen`，按提示完成 OAuth 授权

**四大核心功能：**

| 功能 | 快捷键 / 操作 | 说明 |
|------|-------------|------|
| 代码补全 | `Tab` / `Alt+Shift` | 实时上下文感知补全 |
| 代码生成 | AI聊天面板输入需求 | 自然语言→可运行代码 |
| 代码解释 | 选中代码→提问"逐行解释" | 中文逐行注释 |
| 调试辅导 | 粘贴报错信息→提问 | 中文诊断+修复建议 |

---

## 📊 医学数据集说明

本书各章节均使用**公开可获取**的医学数据集，详见附录B。部分代表性数据集如下：


| 数据集 | 章节                       | 任务类型           | 数据类型 | 样本规模 | 来源 |
|--------|--------------------------|----------------|----------|----------|------|
| **Cleveland 心脏病数据集** | 第4章·有监督学习、第6章半监督学习       | 二分类（心脏病预测）     | 结构化临床数据 | 303 条 | UCI Machine Learning Repository |
| **Wisconsin 乳腺癌诊断数据集** | 第5章·无监督学习                | 二分类（良恶性区分）     | 结构化细胞核特征数据 | 569 条 | UCI Machine Learning Repository |
| **Pima 糖尿病数据集** | 第3章·Python 基础语法与医学AI编程实践 | 二分类（糖尿病预测）     | 结构化临床数据 | 768 条 | UCI / NIDDK |
| **PneumoniaMNIST 肺炎诊断数据集** | 第8章·卷积神经网络               | 二分类（肺炎 vs. 正常） | 胸部X射线图像（28×28） | 5,856 张 | MedMNIST v2 |
| **ISIC 2018 皮肤病变数据集** | 第8章·卷积神经网络               | 皮肤镜图像分割        | 10,015 张 | ISIC Archive |

> ⚠️ **数据使用声明**：本仓库所用数据集均来自公开学术数据源，仅用于教学目的。涉及患者隐私的原始数据不在本仓库存储，使用前请遵守各数据集的许可协议。


---

## 📄 许可证

本仓库代码采用 [MIT License](LICENSE) 开源协议。教材文字内容版权归上海交通大学医学院医学技术学院所有，未经授权不得转载。

---

<div align="center">

**上海交通大学医学院医学技术学院**

*College of Health Science and Technology, Shanghai Jiao Tong University School of Medicine*

</div>
