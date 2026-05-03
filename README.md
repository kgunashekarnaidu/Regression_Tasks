# ElasticNet Grid Search Model

## Overview

This project demonstrates the implementation of an **ElasticNet Regression Model** with **Grid Search Cross Validation** using Python and Scikit-learn. The notebook focuses on building a machine learning pipeline for predicting prices based on multiple input features.

The project includes:

* Data loading and preprocessing
* Feature scaling using StandardScaler
* Train-test data splitting
* ElasticNet regression model building
* Hyperparameter tuning using GridSearchCV
* Model evaluation using regression metrics

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook

---

## Project Workflow

### 1. Data Loading

The dataset is imported and explored using Pandas.

### 2. Feature and Target Separation

* Independent variables (`X`) are separated from the target variable (`y`).
* The target variable used in this project is:

  * `price in $`

### 3. Train-Test Split

The dataset is divided into training and testing sets using:

* `70%` training data
* `30%` testing data

### 4. Feature Scaling

Feature scaling is applied using `StandardScaler` to normalize the data before training the model.

### 5. ElasticNet Regression

An ElasticNet model is created using Scikit-learn.

ElasticNet combines:

* **Lasso Regression (L1 Regularization)**
* **Ridge Regression (L2 Regularization)**

This helps improve model generalization and reduce overfitting.

### 6. Hyperparameter Tuning with GridSearchCV

Grid Search Cross Validation is used to find the best combination of:

* `alpha`
* `l1_ratio`

The model uses:

* `10-fold Cross Validation`
* `Negative Mean Squared Error` as the scoring metric

### 7. Model Evaluation

The trained model is evaluated using:

* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

---

## Model Performance

* Average prediction error: **~$3251**
* R² Score: **0.85**

The model explains approximately **85% of the variance** in the dataset, indicating strong predictive performance.

---

## Repository Structure

```bash
├── Elasticnet Grid Search model.ipynb
├── README.md
```

---

## How to Run the Project

### Clone the Repository

```bash
git clone <your-repository-link>
```

### Install Dependencies

```bash
pip install pandas numpy scikit-learn jupyter
```

### Run the Notebook

```bash
jupyter notebook
```

Open the notebook file and execute the cells sequentially.

---

## Learning Outcomes

Through this project, you can understand:

* Regression modeling
* Data preprocessing techniques
* Feature scaling
* Hyperparameter tuning
* Cross validation
* Performance evaluation of machine learning models

---

## Future Improvements

* Add data visualization for better insights
* Compare ElasticNet with other regression algorithms
* Deploy the trained model using Flask or Streamlit
* Automate the ML pipeline

