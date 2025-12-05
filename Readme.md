# Customer Churn Prediction using PyCaret

This project utilizes **PyCaret**, an open-source, low-code machine learning library in Python, to predict customer churn for a bank. The goal is to identify customers who are likely to leave the bank (`Exited = 1`) based on their demographic and financial activity.

## 📌 Project Overview

Customer churn is a critical metric for banking institutions. This project automates the machine learning workflow to find the best model for predicting churn.

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

## ⚙️ Methodology

1.  **Preprocessing:** Handling missing values and applying SMOTE for class imbalance.
2.  **Model Selection:** Compared multiple models; **Extra Trees Classifier** performed best.
3.  **Results:** Achieved **92.33% Accuracy** and **0.9769 AUC**.

## 🚀 How to Run

1.  Clone the repository.
2.  Install dependencies: `pip install pycaret pandas`
3.  Open the Jupyter Notebook and run all cells to train the model.

## 👤 Author

**Ishaan Vashisth**
* Department of Computer Science and Engineering
* Thapar Institute of Engineering and Technology