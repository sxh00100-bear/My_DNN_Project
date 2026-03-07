# 🚀 My DNN Project: 从古典炼丹到现代视觉

[![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/)
[![TensorFlow 2.x](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://tensorflow.org/)

这是我的深度学习进化之路。记录了从最基础的全连接网络（Dense）到复杂的卷积神经网络（CNN）的探索过程。

---

## 📅 学习进度地图 (Roadmap)

| 章节 | 内容主题 | 状态 | 核心成果 |
| :--- | :--- | :---: | :--- |
| **Ch 01-10** | 机器学习基础与 Keras 入门 | ✅ | 泰坦尼克号、房价预测实战 |
| **Ch 11** | 深度神经网络训练技巧 | ✅ | Batch Normalization、LR Finder |
| **Ch 14** | **深度计算机视觉 (CNN)** | 🏗️ | **CIFAR-10 识别 (当前攻坚点)** |

---

## 🔬 核心实验展示

### 1. CIFAR-10 降维打击
* **实验描述**: 比较 20 层全连接网络与 3 层卷积神经网络的性能差异。
* **关键结论**: 
    * 古典网络准确率瓶颈：**~47%** (无论怎么加深都没用)
    * CNN 初试战果：**~70%+** (引入空间特征抓取)

### 2. CNN 模型架构 (Architecture)
```python
# 核心结构快照
model = keras.models.Sequential([
    keras.layers.Conv2D(64, 3, activation="relu", padding="same"),
    keras.layers.MaxPooling2D(2),
    # ... 更多细节请查看代码文件
])