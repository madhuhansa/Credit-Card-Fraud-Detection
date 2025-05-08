# Credit Card Fraud Detection

This project utilizes a machine learning model to detect fraudulent credit card transactions.

## 📊 Dataset

- **Source**: [Credit Card Fraud Detection Dataset 2023 on Kaggle](https://www.kaggle.com/datasets/nelgiriyewithana/credit-card-fraud-detection-dataset-2023)
- **Features**:
  - `id`: Unique identifier for each transaction
  - `V1` to `V28`: Anonymized transaction features
  - `Amount`: Transaction amount
  - `Class`: 0 = Non-Fraud, 1 = Fraud

## ✅ Model Performance

- **Accuracy**: 100%
- **Precision / Recall / F1-score**: 1.00 for both classes (fraud and non-fraud)

## 🧠 How It Works

The model learns patterns in transaction data and classifies them as fraudulent or legitimate.

## 💾 Saved Model

The trained model is saved using `joblib`:

```python
import joblib
joblib.dump(model, 'model/credit_card_fraud_model.pkl')
```

## 🚀 How to Use

1. Load the saved model:
    ```python
    import joblib
    model = joblib.load('model/credit_card_fraud_model.pkl')
    ```

2. Predict on new data:
    ```python
    prediction = model.predict(new_data)
    ```

## 📁 Folder Structure

```
credit-card-fraud/
├── model/
│   └── credit_card_fraud_model.pkl
├── main.py
├── README.md
```

---

🔒 This model can assist in early fraud detection and prevention in real-time financial systems.
