# 基于多层感知机神经网络的混凝土强度预测

**课程：** 神经网络及其应用  
**学院：** 微电子学院  
**学号：** BC25219017  
**姓名：** 宋城啸  
**日期：** 2026.3.28

---

## 项目简介

本项目基于 [UCI Concrete Compressive Strength Dataset](http://archive.ics.uci.edu/dataset/165/concrete+compressive+strength)，采用结合**主成分分析（PCA）**与**多层感知机（MLP）神经网络**的方法，对混凝土抗压强度进行预测。

传统抗压强度检测依赖物理试验，存在成本高、周期长等问题。本研究利用神经网络模型自主学习混凝土多组分配合比的非线性特征，提高预测精度，为工程配合比设计与强度快速预测提供支持。

## 数据集

| 特征 | 说明 |
|------|------|
| Cement | 水泥用量 (kg/m³) |
| Slag | 矿渣用量 (kg/m³) |
| FlyAsh | 粉煤灰用量 (kg/m³) |
| Water | 水用量 (kg/m³) |
| Superplasticizer | 减水剂用量 (kg/m³) |
| CoarseAggregate | 粗骨料用量 (kg/m³) |
| FineAggregate | 细骨料用量 (kg/m³) |
| Age | 龄期 (天) |
| **Strength** | **混凝土抗压强度（目标变量，MPa）** |

数据集共 1030 条样本，8 个输入特征，1 个输出变量。

## 文件结构

```
.
├── README.md                          # 项目说明文件
├── BC25219017-宋城啸-第一次作业.ipynb  # 主作业 Notebook
├── Concrete_Data_Yeh.csv              # 数据集
└── Homework1.pdf                      # 作业说明文档
```

## 主要方法

1. **数据预处理**：标准化处理、缺失值检查
2. **探索性数据分析（EDA）**：特征分布与相关性可视化
3. **主成分分析（PCA）**：降维与特征提取
4. **MLP 神经网络建模**：多层感知机回归预测
5. **模型评估**：使用 MSE、MAE、R² 等指标评价模型性能

## 环境依赖

- Python 3.x
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- SciPy

## 关键词

抗压强度预测 · BP 神经网络 · 多层感知机（MLP）· 主成分分析（PCA）
