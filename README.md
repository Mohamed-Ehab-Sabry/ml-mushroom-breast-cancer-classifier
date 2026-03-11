# 📊 Naive Bayes Classifier, Feature Selection & PCA from Scratch

A complete classification pipeline exploring **Naive Bayes**, **feature selection**, and **PCA (implemented from scratch)** across categorical and numerical datasets.

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![NumPy](https://img.shields.io/badge/NumPy-From%20Scratch%20PCA-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

---

## 📖 Table of Contents
- [Objective](#objective)
- [Datasets](#datasets)
- [Experimental Pipeline](#experimental-pipeline)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Team](#team)
- [License](#license)

---

## 🎯 Objective

Understand how **Naive Bayes** works, explore **feature selection** techniques, and study **dimensionality reduction using PCA** (built from scratch with NumPy). Compare their effects on model performance across categorical and numerical datasets.

> ⚠️ **Constraint:** PCA is implemented **entirely from scratch** — `sklearn.decomposition.PCA` is **NOT used**.

---

## 📊 Datasets

| Dataset | Type | Features | Source |
|---------|------|----------|--------|
| Dataset 1 | Categorical / Discrete | TBD | [Source Link](#) |
| Dataset 2 | Numerical / Continuous | TBD | [Source Link](#) |

> See [`data/README.md`](data/README.md) for download instructions and justifications.

---

## 🔬 Experimental Pipeline

Each dataset goes through **three experiments**:

| Experiment | Description | Features Used |
|------------|-------------|---------------|
| **Baseline** | Naive Bayes on all original features | All features |
| **Experiment A** | Feature Selection → Naive Bayes | Selected subset of original features |
| **Experiment B** | PCA (from scratch) → Naive Bayes | Top-k principal components |

### Evaluation Metrics
- ✅ Accuracy
- ✅ Classification Report (Precision, Recall, F1)
- ✅ Confusion Matrix

### Visualizations
- 📊 Confusion matrices (heatmaps)
- 📊 Accuracy bar charts (baseline vs. selection vs. PCA)
- 📊 Scree plot (explained variance by component)

---

## 🗂️ Project Structure

```
naive-bayes-pca-analysis/
├── data/               # Raw & processed datasets
├── notebooks/          # Jupyter notebooks (step-by-step experiments)
│   ├── 01_data_exploration.ipynb
│   ├── 02_baseline_naive_bayes.ipynb
│   ├── 03_feature_selection.ipynb
│   ├── 04_pca_from_scratch.ipynb
│   └── 05_comparative_analysis.ipynb
├── src/                # Reusable Python modules
│   ├── preprocessing.py
│   ├── pca_scratch.py          # ⭐ PCA from scratch (NumPy only)
│   ├── feature_selection.py
│   ├── models.py
│   └── evaluation.py
├── results/            # Figures, tables, saved outputs
├── report/             # Final analysis report
├── configs/            # Configuration files
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

```bash
git clone https://github.com/Mohamed-Ehab-Sabry/naive-bayes-pca-analysis.git
cd naive-bayes-pca-analysis
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

---

## 🚀 Usage

Run the notebooks in order:
```bash
jupyter notebook
# Open notebooks/ and run 01 → 02 → 03 → 04 → 05
```

Or run modules directly:
```bash
python -m src.models          # Train Naive Bayes classifiers
python -m src.pca_scratch     # Run PCA from scratch
```

---

## 📈 Results

> Results will be populated after experiments are complete.

| Dataset | Baseline Acc. | Feature Selection Acc. | PCA Acc. (best k) |
|---------|--------------|----------------------|-------------------|
| Dataset 1 (Categorical) | — | — | — |
| Dataset 2 (Numerical) | — | — | — |

See [`results/`](results/) for full figures and [`report/report.md`](report/report.md) for analysis.

---

## 👥 Team

| Name | Role | GitHub |
|------|------|--------|
| Mohamed Ehab | Lead | [@Mohamed-Ehab-Sabry](https://github.com/Mohamed-Ehab-Sabry) |
| Ayman | Collaborator | [@ayman-n1](https://github.com/ayman-n1) |

---

## 📜 License

This project is licensed under the MIT License — see [LICENSE](LICENSE) for details.
