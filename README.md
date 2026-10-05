# HeartGuard — AI-Based Heart Disease Prediction

## 📌 Overview

**HeartGuard** is a machine learning project that predicts the likelihood of heart disease from structured patient data.

The project demonstrates a complete machine learning workflow, including data preprocessing, exploratory data analysis, classification, model evaluation, feature importance analysis, and reusable prediction.

> **Disclaimer:** This project is developed for educational purposes only. It is not a medical diagnostic system and should not be used for real-world medical decisions.

---

## 🎯 Objective

The main objectives of this project are to:

* Analyze structured medical data.
* Handle missing values and prepare the dataset.
* Build classification models for heart disease prediction.
* Compare Logistic Regression and Random Forest.
* Evaluate models using multiple performance metrics.
* Identify important features used by the Random Forest model.
* Create a reusable prediction function.

---

## 📊 Dataset

The project uses the **UCI Heart Disease Dataset**.

The dataset contains **303 patient records** and **13 input features**.

### Features

| Feature  | Description                          |
| -------- | ------------------------------------ |
| age      | Age of the patient                   |
| sex      | Sex                                  |
| cp       | Chest pain type                      |
| trestbps | Resting blood pressure               |
| chol     | Serum cholesterol                    |
| fbs      | Fasting blood sugar                  |
| restecg  | Resting electrocardiographic results |
| thalach  | Maximum heart rate achieved          |
| exang    | Exercise-induced angina              |
| oldpeak  | ST depression                        |
| slope    | Slope of peak exercise ST segment    |
| ca       | Number of major vessels              |
| thal     | Thalassemia                          |

The original target variable contains multiple classes. It was converted into a binary classification target:

* `0` → No Heart Disease
* `1` → Heart Disease

---

## 🛠️ Technologies Used

* Python
* Google Colab
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Joblib

---

## 🤖 Machine Learning Models

### 1. Logistic Regression

Used as a baseline classification model.

### 2. Random Forest Classifier

Used as the main tree-based classification model.

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC-AUC

---

## 🔄 Methodology

The project follows these steps:

1. Dataset collection
2. Data exploration
3. Missing value handling
4. Target transformation
5. Data visualization
6. Train-test split
7. Feature scaling for Logistic Regression
8. Logistic Regression training
9. Random Forest training
10. Model evaluation
11. Confusion matrix analysis
12. ROC-AUC analysis
13. Feature importance analysis
14. Reusable prediction function
15. Model serialization

---

## 📈 Model Evaluation

Both Logistic Regression and Random Forest were evaluated using multiple classification metrics.

The final comparison is available in the notebook.

The model selection was based on overall performance across Accuracy, Precision, Recall, F1-Score, and ROC-AUC rather than relying on a single metric.

---

## 🔍 Feature Importance

Random Forest feature importance was used to understand which input variables contributed most to the model's predictions.

This provides interpretability into how the trained model uses different patient attributes.

**Note:** Feature importance represents the model's reliance on a feature and does not establish medical causation.

---

## 🧪 Prediction

A reusable prediction function was developed that accepts patient feature values and produces:

* Model prediction
* Predicted probability

Input validation was also included to prevent invalid feature values from being processed.

---

## 📁 Project Structure

```text
HeartGuard-Heart-Disease-Prediction/
│
├── Alpha_Task_4_Heart_Disease_Prediction.ipynb
├── heart_disease_prediction_model.pkl
├── scaler.pkl
└── README.md
```

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/your-username/HeartGuard-Heart-Disease-Prediction.git
```

### 2. Open the notebook

Open:

```text
Alpha_Task_4_Heart_Disease_Prediction.ipynb
```

using Google Colab or Jupyter Notebook.

### 3. Install the required dataset package

```python
!pip install -q ucimlrepo
```

### 4. Run the notebook

Execute the cells sequentially to:

* Load the dataset
* Preprocess the data
* Train the models
* Evaluate performance
* Visualize results
* Generate predictions

---

## 💾 Saved Model

The trained Random Forest model is saved as:

```text
heart_disease_prediction_model.pkl
```

The scaler used for Logistic Regression is saved as:

```text
scaler.pkl
```

---

## 📚 Learning Outcomes

Through this project, I gained practical experience in:

* Medical dataset preprocessing
* Binary classification
* Logistic Regression
* Random Forest
* Feature scaling
* Model evaluation
* Confusion matrices
* ROC curves and ROC-AUC
* Feature importance
* Model serialization
* Building reusable ML prediction functions

---

## 🏆 Internship Task

**Alpha Internship — Machine Learning**

**Task 4: Disease Prediction from Medical Data**

---

## 👨‍💻 Author

**Pradoksh Sowdi**

B.E. — Information Science & Engineering

Machine Learning Intern

---

## ⚠️ Disclaimer

This project is intended strictly for educational and machine learning demonstration purposes.

It does not provide medical advice, diagnosis, or treatment recommendations. Real-world medical decisions should always be made by qualified healthcare professionals.
