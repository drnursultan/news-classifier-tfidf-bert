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

