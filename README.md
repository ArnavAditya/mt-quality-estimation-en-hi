# English → Hindi Machine Translation Quality Estimation (QE)

## 📌 Overview

This project implements a Quality Estimation (QE) model for Machine Translation using XLM-Roberta. The goal is to predict translation quality scores for English → Hindi translations without reference translations.

---

## 🧠 Model Architecture

* Base Model: XLM-Roberta (xlm-roberta-base)
* Task: Regression (predict translation quality score)
* Loss Function: Mean Squared Error (MSE)

---

## ⚙️ Features

* Custom PyTorch Dataset for QE
* Transformer-based regression model
* Training with learning rate scheduler
* Evaluation using RMSE
* Prediction pipeline for unseen data

---

## 📂 Dataset Format

CSV files must contain:

* `src` → Source sentence (English)
* `mt` → Translated sentence (Hindi)
* `score` → Quality score (for training)

---

## 🚀 How to Run

1. Install dependencies:

```id="x2m91c"
pip install -r requirements.txt
```

2. Place dataset inside `data/` folder

3. Run:

```id="3pf7zn"
python main.py
```

---

## 📊 Output

* Model saved at: `outputs/en_hi_qe.pt`
* Predictions saved at: `outputs/en_hi_predictions.csv`

---

## 📈 Evaluation Metric

* RMSE (Root Mean Squared Error)

---

## 🔬 Techniques Used

* Transformer-based embeddings (XLM-R)
* Regression for QE
* Tokenization using HuggingFace

---

## 🔮 Future Work

* Integrate data augmentation techniques
* Extend to full MT pipeline
* Use larger models (XLM-R Large)

---

## 👨‍💻 Author

Arnav Aditya
