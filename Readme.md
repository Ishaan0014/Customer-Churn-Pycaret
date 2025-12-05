# Customer Churn Prediction using PyCaret

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![PyCaret](https://img.shields.io/badge/PyCaret-AutoML-orange?logo=python&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-success)

This project utilizes **PyCaret**, an open-source, low-code machine learning library in Python, to predict customer churn for a bank. The goal is to identify customers who are likely to leave the bank (`Exited = 1`) based on their demographic and financial activity.

## 📌 Project Overview

Customer churn is a critical metric for banking institutions. Retaining existing customers is often more cost-effective than acquiring new ones. This project automates the machine learning workflow to find the best model for predicting churn.

* **Target Variable:** `Exited` (Binary: 1 = Churn, 0 = Retained)
* **Best Model Selected:** Extra Trees Classifier
* **Final Accuracy:** ~92.3%

## 📂 Dataset

The dataset (`Churn_Modelling.csv`) contains details of bank customers. Key features include:

* **Demographics:** Geography, Gender, Age.
* **Financials:** Credit Score, Balance, Estimated Salary.
* **Engagement:** Tenure, Number of Products, Has Credit Card, Is Active Member.

## 🛠️ Tech Stack

* **Python**
* **PyCaret** (AutoML)
* **Pandas** (Data Manipulation)
* **Matplotlib** (Visualization)

## ⚙️ Methodology

1.  **Data Loading:** Ingesting the customer dataset.
2.  **Preprocessing:**
    * Handling missing values (Mean/Mode imputation).
    * **Class Imbalance Handling:** Applied `SMOTE` (Synthetic Minority Over-sampling Technique) to balance the target classes.
3.  **Model Selection:** Compared multiple models using PyCaret's `compare_models()` function. The **Extra Trees Classifier** was identified as the top performer.
4.  **Tuning:** Attempted hyperparameter tuning (base model performed optimally).
5.  **Finalization:** The model was finalized and tested on a hold-out test set.

## 📊 Results

The model performance on the held-out test set was exceptional:

| Metric | Score |
| :--- | :--- |
| **Accuracy** | **92.33%** |
| **AUC** | **0.9769** |
| **Recall** | 0.7021 |
| **Precision** | 0.8994 |
| **F1 Score** | 0.7886 |

### Visualizations

The project includes key visualizations to understand model performance:

**1. Confusion Matrix**
*(Visualizes True Positives and False Negatives)*
![Confusion Matrix](Confusion%20Matrix.png)

**2. Feature Importance**
*(Identifies which factors contribute most to churn)*
![Feature Importance](Feature%20Importance%20Plot.png)

## 🚀 How to Run

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Ishaan0014/Customer-Churn-Pycaret.git](https://github.com/Ishaan0014/Customer-Churn-Pycaret.git)
    ```

2.  **Install dependencies:**
    ```bash
    pip install pycaret pandas
    ```

3.  **Run the Notebook:**
    Open `IshaanVashisth_8025340019_Customer_Churn_ Prediction_Pycaret_Project.ipynb` in Jupyter Notebook or Google Colab and run all cells to train the model.

## 👤 Author

**Ishaan Vashisth**
Department of Computer Science and Engineering
Thapar Institute of Engineering and Technology
