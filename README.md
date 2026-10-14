# DevSecMLOps Lab Projects

Two runnable projects from the DevSecMLOps lab record, each in its own folder with its own
`requirements.txt`, tests and README.

| Folder | Lab experiment | What it does |
|---|---|---|
| [`churn-mlflow/`](churn-mlflow) | Experiment 4 | Customer churn prediction (Logistic Regression, Random Forest, Gradient Boosting) with MLflow experiment tracking |
| [`secure-ml-api/`](secure-ml-api) | Experiment 7 | Flask ML prediction API with API-key authentication, input validation and a health endpoint |

## Quick start

```bash
git clone <this-repo-url> && cd devsecmlops-lab-projects

# Project 1
cd churn-mlflow
python -m venv .venv && source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt
python churn.py
cd ..

# Project 2
cd secure-ml-api
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python app.py --demo
```

GitHub Actions run the tests (and Bandit / pip-audit for the API) for each project whenever its folder changes.
