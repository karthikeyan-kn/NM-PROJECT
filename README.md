# Customer Churn Prediction API

This project deploys a machine learning model to predict customer churn using a Flask API.

## 📁 Files
- `best_rf_model.joblib` — Trained Random Forest model
- `scaler.joblib` — Scikit-learn StandardScaler
- `lda.joblib` — LDA dimensionality reducer
- `churn_api_flask.py` — Flask API script
- `requirements.txt` — Python dependencies

## 🚀 How to Run Locally

1. Install dependencies:
    ```
    pip install -r requirements.txt
    ```

2. Run the Flask server:
    ```
    python churn_api_flask.py
    ```

3. Use a tool like Postman or curl to send a POST request:
    ```
    POST http://127.0.0.1:5000/predict
    Content-Type: application/json

    {
      "features": [1.0, 45.0, 29.5, ...]  # Input must match training feature order
    }
    ```

## 📦 Deployment

You can deploy this repo to Render, Heroku, or Railway.