# ANN Churn Prediction

This repository contains a simple **Artificial Neural Network (ANN)** project for customer churn prediction, along with a small Streamlit app for interactive inference.

## Repository Contents

- `app.py` – Streamlit app to collect user inputs and predict churn probability using a trained model.
- `model.h5` – Trained Keras/TensorFlow model used for predictions.
- `scaler.pkl` – Fitted scaler for numeric feature preprocessing.
- `label_encoder_gender.pkl` – Label encoder for the `Gender` feature.
- `onehot_encoder_geo.pkl` – One-hot encoder for the `Geography` feature.
- `Churn_Modelling.csv` – Dataset file used in model experimentation/training.
- `experiment.ipynb` – Notebook for experimentation/model development.
- `prediction.ipynb` – Notebook focused on prediction workflow.
- `test.py` – Python script present in the repository.
- `requirements.txt` – Python dependencies.
- `runtime.txt` – Runtime/version configuration.

## What the App Does

The Streamlit app:

1. Loads the trained model and preprocessing artifacts.
2. Accepts user inputs (customer profile and account details).
3. Applies the same preprocessing steps used during training.
4. Outputs churn probability and a churn/non-churn message.

## Quick Start

1. Create and activate a virtual environment.
2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run the app:

```bash
streamlit run app.py
```

## Notes

- Keep `model.h5` and all `.pkl` files in the project root so `app.py` can load them correctly.
- This is a baseline project structure and can be extended with better validation, testing, and deployment setup.
