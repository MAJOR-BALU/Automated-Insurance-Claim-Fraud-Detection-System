# Insurance Claim Fraud Detection Dashboard

This project is a machine learning-based dashboard for detecting potential fraud in insurance claims. It combines supervised classification with anomaly detection to identify and flag high-risk claims. The dashboard is interactive and built using Streamlit.

## Features

- Preprocessing and label encoding of insurance claim data
- SMOTE-based oversampling to handle class imbalance
- Grid search with cross-validation for hyperparameter tuning
- Random Forest classifier for supervised fraud prediction
- Isolation Forest for anomaly-based fraud scoring
- Combined risk score based on prediction and anomaly metrics
- Top 10% most suspicious claims automatically flagged
- Dashboard visualization with full claim-level data

## Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- imbalanced-learn (SMOTE)
- Streamlit
- Jupyter Notebook

## Folder Structure

```
fraud_detection_project/
├── data/
│   └── insurance_claims.csv       # Input dataset
│   └── risk_scores.csv            # Generated after training
│   └── auc.txt                    # Model performance metric
├── notebook/
│   └── fraud_analysis.ipynb       # Jupyter Notebook for model training
├── app/
│   └── dashboard.py               # Streamlit app code
├── requirements.txt               # Python dependencies
└── README.md                      # Project documentation
```

## How to Run

1. Clone or download the project folder.
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook:
   ```bash
   cd notebook
   jupyter notebook
   ```
   Open `fraud_analysis.ipynb` and run all cells to generate model outputs.
4. Launch the Streamlit dashboard:
   ```bash
   cd ../app
   streamlit run dashboard.py
   ```

