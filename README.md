# 📰 Multi-Level News Classifier — TF-IDF vs BERT

This project compares two text classification approaches on the **AG News dataset**:
1. **Baseline:** TF-IDF + Logistic Regression  
2. **Advanced:** Fine-tuned BERT (`bert-base-uncased`)  

---

## 📊 Dataset
The [AG News dataset](https://www.kaggle.com/datasets/amananandrai/ag-news-classification-dataset) contains **4 categories**:
- World  
- Sports  
- Business  
- Sci/Tech  

Each record has a *Title* and *Description* column.

---

## 📁 Project Structure

```
news-classifier/
├── data/
│   ├── train.csv
│   └── test.csv
├── notebooks/
│   ├── 01_eda.html
│   ├── 02_baseline_tfidf.html
│   └── 03_bert_finetune_clean.html
├── reports/
│   ├── conf_matrix_tfidf.png
│   └── conf_matrix_bert.png
└── README.md
```

---

## 📘 Notebooks (clickable)

| Notebook | Description |
|-----------|--------------|
| [01_eda.html](notebooks/01_eda.html) | Exploratory Data Analysis |
| [02_baseline_tfidf.html](notebooks/02_baseline_tfidf.html) | TF-IDF Baseline Model |
| [03_bert_finetune_clean.html](notebooks/03_bert_finetune_clean.html) | Fine-Tuned BERT Model |

---

## 🧠 Model Comparison

| Metric | TF-IDF + Logistic Regression | BERT (Fine-Tuned) |
|:-------|:-----------------------------:|:-----------------:|
| Accuracy | **0.92** | **0.95** |
| Precision (avg) | 0.92 | 0.95 |
| Recall (avg) | 0.92 | 0.95 |
| F1-Score (avg) | 0.92 | 0.95 |
| Training Epochs | – | 2 |
| Training Loss (last) | – | 0.1120 |
| Validation Loss (last) | – | 0.1886 |

---

## 📈 Confusion Matrices

| TF-IDF | BERT |
|:------:|:----:|
| ![TF-IDF Confusion Matrix](reports/conf_matrix_tfidf.png) | ![BERT Confusion Matrix](reports/conf_matrix_bert.png) |

---

## 🧩 Evaluation Reports

### BERT Report
```
          precision    recall  f1-score   support

   World       0.96      0.96      0.96      1900
  Sports       0.99      0.99      0.99      1900
Business       0.93      0.91      0.92      1900
Sci/Tech       0.91      0.94      0.92      1900

accuracy                           0.95      7600

```
