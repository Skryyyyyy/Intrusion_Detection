# IoT Intrusion Detection Using Machine Learning

## Project Overview

This project implements an IoT Intrusion Detection System using machine learning to classify network traffic as Normal or Attack and categorize traffic into eight broader classes.

## Algorithms Used

- **Decision Tree Classifier:** Baseline model.
- **Random Forest Classifier:** Ensemble of 100 decision trees.

## Technologies

- Python
- Pandas and NumPy
- Scikit-learn
- Matplotlib and Seaborn
- Joblib
- Jupyter Notebook

## Project Structure

```text
MLCS/
├── models/
│   ├── feature_columns.json
│   ├── rf_binary_model.joblib
│   └── rf_category_model.joblib
├── IoT_Intrusion_Detection_Complete_Serialization_Reusability.ipynb
├── README.md
└── requirements.txt
```

## Model Serialization and Reusability

The trained Random Forest models are saved using Joblib.

- `rf_binary_model.joblib`: Predicts Normal versus Attack.
- `rf_category_model.joblib`: Predicts one of eight traffic categories.
- `feature_columns.json`: Stores the expected input feature names and order.

The saved models can be loaded and reused for prediction without retraining.

## How to Run

Install dependencies:

```bash
pip install -r requirements.txt
```

Open the Jupyter Notebook and execute its cells in order. Ensure the dataset `IoT_Intrusion.csv` is available locally in the expected location.

## Evaluation

The notebook evaluates the models using accuracy, precision, recall, F1-score, classification reports, and confusion matrices.

## Conclusion

This project demonstrates IoT traffic classification, model evaluation, serialization, and reusability of trained machine learning models.
