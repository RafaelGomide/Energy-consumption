# ⚡️ Building Energy Consumption Prediction 🏠

## Project Overview

This project presents a Machine Learning model designed to predict the **Energy Consumption** of a building based on various structural and environmental factors. The model uses an **XGBoost Regressor**, a powerful gradient boosting framework, to achieve high prediction accuracy.

The dataset used for this project was **created by the author**, inspired by the well-known *Energy Consumption - Linear Regression* dataset available on Kaggle. This ensures a realistic yet controlled environment for model training and evaluation.

## ✨ Key Features

- **Data Generation:** A synthetic dataset of 10,000 records is generated using `numpy` and `pandas`, simulating real-world building characteristics and energy usage.

- **Feature Engineering:** Categorical variables like `Building Type` and `Day of Week` are handled using one-hot encoding (`pd.get_dummies`).

- **Advanced Regression Model:** Utilizes the **XGBoost Regressor** for robust and accurate energy consumption prediction.

- **Model Evaluation:** Performance is tracked using **Root Mean Squared Error (RMSE)** on both training and validation sets, demonstrating low error and good generalization.

## 📊 Dataset Structure

The synthetic dataset contains 7 columns:

| Feature | Data Type | Description |
| --- | --- | --- |
| `Building Type` | Categorical | Residential, Commercial, or Industrial. |
| `Square Footage` | Integer | The size of the building in square feet. |
| `Number of Occupants` | Integer | The number of people in the building. |
| `Appliances Used` | Integer | The number of major appliances in use. |
| `Average Temperature` | Float | The average outside temperature in Celsius. |
| `Day of Week` | Categorical | Weekday or Weekend. |
| `Energy Consumption` | Float | **Target Variable:** The predicted energy consumption. |

## 🚀 Getting Started

### Prerequisites

To run this project, you need Python and the following libraries:

```bash
pip install pandas numpy scikit-learn xgboost matplotlib
```

### Running the Notebook

1. **Clone the repository** (assuming this is a repository):

1. **Open the Jupyter Notebook:**

1. **Run all cells** in the notebook to generate the data, train the model, and view the results.

## 📈 Model Performance

The model was trained and evaluated using a train-test split, with performance measured by the **Root Mean Squared Error (RMSE)**.

| Metric | Training Set | Validation Set |
| --- | --- | --- |
| **Final RMSE** | ~481.55 | ~503.77 |

The low and closely matched RMSE values indicate that the model is highly accurate and generalizes well to unseen data, with minimal signs of overfitting.

## 💡 Inspiration and Data Source

The concept for this project and the structure of the synthetic dataset were **inspired by the Energy Consumption - Linear Regression dataset available on Kaggle**. The data itself was custom-generated to provide a controlled and educational environment for demonstrating the power of the XGBoost Regressor in a regression task.

## 🧑‍💻 Author

[Rafael Gomide]

---

*This README was generated to showcase the project's technical depth and visual appeal.*

