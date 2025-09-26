# 📰 Fake News Detection  

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg) | ![Jupyter](https://img.shields.io/badge/Notebook-Jupyter-orange.svg) | ![License: MIT](https://img.shields.io/badge/License-MIT-green.svg) | ![Build](https://img.shields.io/badge/Build-Passing-brightgreen.svg)  

A machine learning project that trains and evaluates a **fake news classification model** from tabular text data using **Jupyter Notebooks**. The workflow demonstrates industry best practices for reproducible ML development — including data preprocessing, feature engineering, cross-validation, and pipeline-based model training.  

---

## 📂 Project Structure  
FakeNews-Detection/
│
├── data/ # Dataset (download separately)
├── notebooks/
│ ├── Untitled.ipynb # Baseline workflow
│ ├── Untitled_optimized.ipynb # Reproducible + CV/Pipeline version
├── requirements.txt # Project dependencies
├── README.md # Documentation

---

## ⚙️ Features  

- Data loading & cleaning  
- Feature engineering & encoding  
- **Stratified** train/validation/test splits  
- Model training with **scikit-learn Pipelines** (avoiding leakage)  
- Cross-validated evaluation (Accuracy, F1, Confusion Matrix)  
- Optional **hyperparameter search** (GridSearchCV / RandomizedSearchCV)  
- Reproducibility with fixed seeds  
- Lightweight profiling/timers for faster iterations  

---

## 📊 Dataset  

This project uses the **Fake News Dataset** from Kaggle:  
🔗 [Fake News Dataset (Kaggle)](https://www.kaggle.com/c/fake-news/data)  

Download and place the CSV file(s) inside the `data/` folder before running the notebooks.  

---

## 🚀 Getting Started  

### 1. Clone the repo  
```bash
git clone https://github.com/GauravP1101/FakeNews-Detection.git
cd FakeNews-Detection

2. Create & activate a virtual environment
python -m venv .venv
# Windows
.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate

3. Install dependencies
pip install -r requirements.txt

If requirements.txt is missing, you can start with:

pip install jupyter numpy pandas scikit-learn matplotlib seaborn xgboost lightgbm catboost
pip freeze > requirements.txt

4. Run notebooks
jupyter notebook

🛠️ Tech Stack

Python 3.9+

Pandas, NumPy, Scikit-learn

XGBoost, LightGBM, CatBoost

Jupyter Notebook

Matplotlib / Seaborn

📌 Next Steps

Extend with deep learning models (LSTM / BERT)

Deploy as an API using FastAPI / Flask

Build an interactive UI with Streamlit / Gradio

