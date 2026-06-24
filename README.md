# 🧠 Neural Network Assignment — Shallow vs Deep NN

A complete machine learning pipeline comparing a **Shallow Neural Network** and a **Deep Neural Network** on the Pima Indians Diabetes dataset, built with PyTorch inside Google Colab.

---

## 📁 Repository Structure

```
ANN-Assignment/
│
├── diabetes.csv          # Raw dataset (Pima Indians Diabetes)
├── ANN_Assignment.ipynb  # Full Colab notebook (run end-to-end)
└── README.md             # This file
```

---

## 📊 Dataset

| Property | Details |
|----------|---------|
| **Name** | Pima Indians Diabetes Dataset |
| **Source** | [Raw CSV Link](https://raw.githubusercontent.com/plotly/datasets/master/diabetes.csv) |
| **Samples** | 768 |
| **Features** | 8 (Glucose, BMI, Age, etc.) |
| **Target** | Binary — `Outcome` (0 = No Diabetes, 1 = Diabetes) |
| **Task** | Binary Classification |

---

## 🏗️ Model Architectures

### Shallow Neural Network
| Layer | Details |
|-------|---------|
| Input | 8 features |
| Hidden Layer | 32 units — Sigmoid activation |
| Output | 1 unit — Sigmoid activation |
| **Total Parameters** | **321** |

### Deep Neural Network
| Layer | Details |
|-------|---------|
| Input | 8 features |
| Hidden Layer 1 | 128 units — ReLU — Dropout(0.3) |
| Hidden Layer 2 | 64 units — ReLU — Dropout(0.3) |
| Hidden Layer 3 | 32 units — ReLU — Dropout(0.3) |
| Output | 1 unit — Sigmoid activation |
| **Total Parameters** | **11,521** |

---

## 📈 Results

| Metric | Shallow NN | Deep NN |
|--------|-----------|---------|
| **Accuracy** | 70.78% | **75.32%** |
| **Precision** | 0.6000 | **0.6481** |
| **Recall** | 0.5000 | **0.6481** |
| **F1-Score** | 0.5455 | **0.6481** |
| **AUC** | **0.8141** | 0.8101 |

> ✅ The Deep NN outperforms in Accuracy, Precision, Recall, and F1-Score.
> The Shallow NN has a marginally higher AUC (0.8141 vs 0.8101).

---

## 🔬 Pipeline Steps

1. **Data Preprocessing** — Median imputation for zero-values, StandardScaler normalization, stratified 80/20 train-test split
2. **Shallow NN** — 1 hidden layer, hyperparameter tuning over hidden units, activation functions, and batch size
3. **Deep NN** — 3+ hidden layers with Dropout regularization, tuning over learning rate, optimizer (Adam vs SGD), and epochs
4. **Visualizations** — Training history, Confusion Matrix, ROC Curve, grouped metrics bar chart, architecture summary
5. **Analysis** — Critical comparison of both models

---

## 📉 Visualizations Included

| # | Type | Format |
|---|------|--------|
| 1 | Training Loss & Accuracy History | 2×1 Side-by-side |
| 2 | Confusion Matrix (Heatmap) | 2×1 Side-by-side |
| 3 | ROC Curve + AUC Score | 2×1 Side-by-side |
| 4 | All Metrics Grouped Bar Chart | Combined single chart |
| 5 | Network Architecture Summary | Text topology table |

---

## ▶️ How to Run

1. Open the Colab notebook via the link below
2. Go to **Runtime → Run All**
3. The notebook will automatically fetch the dataset from this repository — **no manual uploads needed**

---

## 🔗 Links

| Resource | Link |
|----------|------|
| 📓 Google Colab Notebook | [Open in Colab](https://colab.research.google.com/drive/1PZFojND56vkixhGrDOgbhyqnjJg33BSz?usp=sharing) |
| 📂 GitHub Repository | [View Repo](https://github.com/thrafid/ANN-assignment) |
| 🗄️ Dataset (Raw CSV) | [diabetes.csv](https://raw.githubusercontent.com/thrafid/ANN-assignment/refs/heads/main/diabetes.csv) |

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.x-orange)
![Scikit--learn](https://img.shields.io/badge/Scikit--learn-1.x-green)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-lightblue)
![Colab](https://img.shields.io/badge/Google%20Colab-Ready-yellow)

| Library | Purpose |
|---------|---------|
| `PyTorch` | Building & training neural networks |
| `Scikit-learn` | Preprocessing, metrics, train-test split |
| `Pandas / NumPy` | Data manipulation |
| `Matplotlib / Seaborn` | Visualizations |

---

## 👤 Author

**MD. TAHMIDUL HASAN**,
ID: 220117
