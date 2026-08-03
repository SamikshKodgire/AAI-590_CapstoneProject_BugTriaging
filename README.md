# 🐞 Intelligent Bug Priority Prediction Using Machine Learning and Transformer Models

## 📌 Project Overview

Software maintenance teams often receive thousands of bug reports, making manual bug prioritization a time-consuming and subjective process. Incorrect prioritization can delay the resolution of critical issues and negatively impact software quality.

This project presents an **end-to-end machine learning framework** for automatically predicting the priority of software bug reports using Natural Language Processing (NLP), traditional Machine Learning algorithms, and Transformer-based Deep Learning models.

Bug reports collected from multiple open-source software repositories were preprocessed, analyzed, and modeled to classify bugs into five unified priority levels.

The project was developed as part of the **Master of Science in Applied Artificial Intelligence** program at the **University of San Diego**.

---

# 🎯 Objectives

The primary objectives of this project are to:

- Automate software bug priority prediction using AI.
- Compare traditional Machine Learning and Transformer-based approaches.
- Develop a reproducible end-to-end NLP pipeline.
- Evaluate multiple models using standard classification metrics.
- Demonstrate the trade-offs between predictive performance and computational cost.
- Provide dashboard-ready outputs for business intelligence and visualization.

---

# 📊 Dataset

The project utilizes publicly available bug reports collected from multiple open-source software repositories.

### Data Sources

- Git Bugs Dataset (Kaggle)
- Bugzilla Eclipse Bug Reports Dataset (Hugging Face)

The original repository-specific priority labels were standardized into five unified classes:

- Critical
- High
- Medium
- Low
- Very Low

---

# 🛠️ Project Workflow

```
Data Collection
        │
        ▼
Data Quality Assessment
        │
        ▼
Exploratory Data Analysis
        │
        ▼
Data Cleaning
        │
        ▼
NLP Preprocessing
        │
        ▼
TF-IDF Feature Engineering
        │
        ▼
Traditional Machine Learning
(Logistic Regression,
 Random Forest,
 XGBoost)
        │
        ▼
Transformer Fine-Tuning
(DistilBERT)
        │
        ▼
Model Comparison
        │
        ▼
Interactive Dashboard Export
```

---

# 🤖 Models Implemented

The following models were developed and evaluated:

| Model | Purpose |
|--------|----------|
| Logistic Regression | Baseline classifier |
| Random Forest | Ensemble learning |
| XGBoost | Gradient boosting |
| DistilBERT | Transformer-based deep learning |

---

# 📈 Model Performance

| Model | Accuracy | Weighted F1 | ROC-AUC |
|--------|---------:|------------:|--------:|
| Logistic Regression | 69.39% | 70.62% | 92.57% |
| Random Forest | **75.16%** | **73.17%** | **92.73%** |
| XGBoost | 74.40% | 71.59% | 92.62% |
| DistilBERT | 74.65% | 72.40% | 92.67% |

### Key Findings

- Random Forest achieved the highest overall predictive performance.
- DistilBERT demonstrated competitive performance while leveraging contextual language representations.
- Traditional TF-IDF features combined with ensemble learning remained highly effective for this dataset.
- Transformer models eliminated manual feature engineering and provided a scalable NLP solution.

---

# 📁 Repository Structure

```
├── notebooks/
│   └── Intelligent_Bug_Priority_Prediction.ipynb
│
├── checkpoints/
│
├── models/
│
├── results/
│
├── dashboard_data/
│
├── README.md
│
└── requirements.txt
```

---

# 📦 Technologies Used

### Programming Language

- Python 3.12

### Data Processing

- Pandas
- NumPy

### Machine Learning

- Scikit-learn
- XGBoost

### Deep Learning

- PyTorch
- Hugging Face Transformers

### Visualization

- Matplotlib
- Seaborn
- Tableau

### Utilities

- Joblib
- Datasets

---

# 📊 Dashboard

The project exports dashboard-ready datasets that can be directly imported into Tableau or Microsoft Power BI.

The dashboard includes:

- Executive KPI Cards
- Priority Distribution
- Repository-wise Analysis
- Model Performance Comparison
- Performance vs Computational Cost
- Interactive Filtering

---

# 🚀 How to Run

1. Clone the repository.

```bash
git clone https://github.com/<your-username>/Intelligent-Bug-Priority-Prediction.git
```

2. Install dependencies.

```bash
pip install -r requirements.txt
```

3. Open the Jupyter notebook.

```bash
jupyter notebook
```

4. Execute the notebook sequentially.

---

# 📚 References

- Breiman, L. (2001). *Random Forests.*
- Chen, T., & Guestrin, C. (2016). *XGBoost: A Scalable Tree Boosting System.*
- Devlin, J., et al. (2019). *BERT: Pre-training of Deep Bidirectional Transformers.*
- Sanh, V., et al. (2019). *DistilBERT.*
- Pedregosa, F., et al. (2011). *Scikit-learn: Machine Learning in Python.*
- Jurafsky, D., & Martin, J. H. *Speech and Language Processing.*

---

# 👩‍💻 Author

**Samiksha Kodgire**
**Manoj Nair**

Master of Science in Applied Artificial Intelligence  
University of San Diego

---

# 📄 License

This repository is intended for academic and educational purposes as part of a graduate-level capstone project.
