# AI-Powered Financial Fraud Detection System
Python | Random Forest | XGBoost | SMOTE | Streamlit

## Run
    python generate_data.py     # synthetic data -> data/transactions.csv (skip if you have a real dataset)
    python train.py             # features + SMOTE + RF/XGBoost -> models/, reports/
    streamlit run app.py        # dashboard

## Method
- Leak-safe feature engineering (user history, 24h velocity, time features)
- Time-based train/test split; SMOTE applied only inside the training pipeline
- Metrics: ROC-AUC, PR-AUC, recall, precision; threshold tuned for recall
