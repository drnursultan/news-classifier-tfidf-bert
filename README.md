# Multi-Level News Classifier (TF-IDF vs BERT)

This project compares two text classification approaches on the AG News dataset:
1. **TF-IDF + Logistic Regression** (classical baseline)
2. **Fine-tuned BERT (bert-base-uncased)** for contextual understanding.

### Dataset
AG News dataset (4 categories: World, Sports, Business, Sci/Tech).

### Notebooks
- `01_eda.html` — Exploratory Data Analysis
- `02_baseline_tfidf.html` — TF-IDF baseline model
- `03_bert_finetune_clean.html` — Fine-tuned BERT model

### Results
| Model | Accuracy | Notes |
|--------|-----------|-------|
| TF-IDF | ~90% | Fast but ignores word context |
| BERT | ~94% | Context-aware, slower but more accurate |

### How to Run
Run notebooks sequentially in Google Colab or Jupyter. BERT training requires GPU.
