# **ML for Predicting Hematological Activity in APS Patients**

This repository contains the Jupyter notebook `pAPS.ipynb`, which uses machine learning classifiers to predict **hematological activity** in **Antiphospholipid Syndrome (APS)** patients. This project leverages clinical and laboratory data to improve predictions and incorporates **SHAP (SHapley Additive exPlanations)** to explain model predictions.

## **Overview**

APS is a disorder that can cause abnormal blood clotting, leading to various clinical complications. This project aims to predict the **hematological activity** in APS patients using ML classifiers such as **Gradient Boosting Machine (GBM)** and **XGBoost**. The project also explores the importance of various clinical features using SHAP values.

## **Data**

The dataset used in this project contains clinical and laboratory information of APS patients. Features include both numerical and categorical variables that are used to train the models.

### **Features:**
- **Numerical Features:** Age at diagnosis, platelet count, lymphocyte count, etc.
- **Categorical Features:** Gender, anticoagulation therapy type, etc.
- **Target Variable:** Hematological activity (binary classification).

## **Models Used**

- **Gradient Boosting Machine (GBM)**
- **XGBoost**
- **SVM**
- **Logistic Regression**

## **Installation**

1. **Clone the repository:**
 
   ```bash
   git clone https://github.com/aquinteroville/ML-for-APS.git
   cd ML-for-APS

2. **Install the required dependencies:**
   - Create a virtual environment and install the necessary Python packages:
     ```bash
     python -m venv env
     source env/bin/activate  # On Windows use `env\Scripts\activate`
     pip install -r requirements.txt
     ```
   - If no `requirements.txt` is provided, install the necessary libraries manually:
     ```bash
     pip install pandas numpy scikit-learn shap matplotlib xgboost
     ```
## **Usage**

1. **Open the Jupyter notebook:**
   You can launch the notebook by running the following command:
   ```bash
   jupyter notebook pAPS.ipynb

2. **Run the notebook:** Execute the cells to perform data preprocessing, model training, evaluation, and SHAP analysis.

3. **Visualize SHAP values:** The notebook will generate SHAP value plots to explain model predictions and feature importance.

## **Project Structure**

- `pAPS_.ipynb`: The main Jupyter notebook containing the data preprocessing, machine learning model training, evaluation metrics, and SHAP analysis.
- `data/`: Placeholder for data files (data not included due to privacy concerns).
- `README.md`: This README file.

## **Model Explanations Using SHAP**

After training the models, SHAP is used to explain the contribution of each feature to the predictions. The SHAP plots highlight the most significant clinical variables influencing hematological activity predictions.

### **SHAP Analysis Includes:**

- **SHAP Summary Plot:** Displays the most impactful features across the dataset.
- **SHAP Force Plot:** Visualizes the contribution of features to individual predictions.

## **Contributing**

If you'd like to contribute to this project, feel free to fork the repository and submit a pull request.

## **License**

This project is licensed under the MIT License. For more details, see the LICENSE file.

## **Acknowledgments**

Thank you to everyone involved in the development of this project.
