# SHAP Feature Importance Project

## 🎯 Project Overview
This project aims to build, evaluate, and interpret two different XGBoost regression models on a dataset using SHAP values. The goal is to identify the most influential features affecting model predictions.

### 📌 Key Features
- **Data preprocessing pipeline** (numerical scaling, ordinal, and one-hot encoding)
- **Two different XGBoost models** with varying hyperparameters
- **Performance evaluation** (MAE, MSE, R²)
- **SHAP interpretation** for global and local feature importance

---

## 🛠️ Installation
Ensure you have Python installed (>=3.8), then install the required packages with:

```bash
pip install -r requirements.txt
```

---

## 📁 Project Structure
```plaintext
/your_project_folder
│
├── students.ipynb          # Jupyter Notebook containing the code
├── readme.md                # Project documentation (this file)
└── requirements.txt         # List of required packages
```

---

## 🔧 How to Run

1. **Load the dataset:** Ensure the dataset is loaded into `X` (features) and `y` (target).
2. **Define pipelines:** Set up preprocessing steps and model configurations.
3. **Train both models:** Run `pipeline_1.fit()` and `pipeline_2.fit()`.
4. **Evaluate performance:** Check MAE, MSE, and R² for each model.
5. **Apply SHAP:**
   - Generate SHAP values
   - Analyze global feature importance (`summary_plot`)
   - Display average importance (`bar`)
   - Dive into specific predictions (`force_plot`)

---

## 📊 Model Comparison
Two pipelines are defined:

- **Model 1:** `max_depth=3`, `learning_rate=0.1`, `n_estimators=100`
- **Model 2:** `max_depth=7`, `learning_rate=0.01`, `n_estimators=500`

Performance metrics are printed for each model, allowing you to compare accuracy.

---

## 🔍 SHAP Insights
SHAP explanations provide a breakdown of how each feature contributes to the model's prediction.

- **Summary plot:** Shows the global impact of all features.
- **Bar plot:** Displays average feature importance.
- **Force plot:** Explains an individual prediction.

---

## 🔥 Future Improvements
- **Hyperparameter tuning** with GridSearchCV
- **Cross-validation** for more robust performance evaluation
- **Handling missing data** with imputation strategies
- **Comparative SHAP analysis** between the two models

---

🚀 **Happy modeling and interpreting with SHAP!**