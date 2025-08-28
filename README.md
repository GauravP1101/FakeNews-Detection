This repo trains and evaluates a classification model from tabular data using a single Jupyter Notebook. It covers:

Data loading & cleaning

Feature engineering & encoding

Train/validation/test splits with stratification

Model training with pipelines (no leakage)

Cross-validated evaluation (accuracy, F1, confusion matrix)

Optional hyperparameter search (GridSearchCV / RandomizedSearchCV)

Reproducible runs (fixed seeds)

Lightweight profiling/timers for faster iterations

There are two notebooks:

notebooks/Untitled.ipynb — original workflow

notebooks/Untitled_optimized.ipynb — instrumented for reproducibility, timing, and CV/Pipeline best practices.

🛠️ Setup

Python ≥ 3.9 is recommended.

# 1) Create & activate a virtual environment
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

# 2) Install dependencies
pip install -r requirements.txt

# If you don't have requirements.txt yet, start with:
pip install jupyter numpy pandas scikit-learn matplotlib seaborn xgboost lightgbm catboost
pip freeze > requirements.txt





