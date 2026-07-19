# 🧩 Column Transformer in Machine Learning

## 📌 Overview

This project demonstrates how to use **ColumnTransformer** in Scikit-learn to preprocess different types of features in a dataset.

Real-world datasets often contain both **numerical** and **categorical** columns. Since these columns require different preprocessing techniques, `ColumnTransformer` allows us to apply separate transformations to different column groups in a single preprocessing pipeline.

This project uses the **Titanic Dataset** to predict passenger survival using Logistic Regression after preprocessing the data.

---

# 📂 Dataset

**Dataset:** Titanic Dataset

Target Column:
- Survived

Features:
- Pclass
- Sex
- Age
- Fare
- Embarked

---

# 🎯 Project Objective

The objective of this project is to learn how to preprocess mixed data types efficiently using **ColumnTransformer** and integrate preprocessing with a machine learning model using **Pipeline**.

---

# 📚 What is ColumnTransformer?

`ColumnTransformer` is a Scikit-learn class used to apply different preprocessing techniques to different columns of a dataset.

Instead of manually transforming each column separately, it allows multiple preprocessing steps to be performed in a single workflow.

Example:

Numerical Columns
- Age
- Fare

Categorical Columns
- Sex
- Embarked
- Pclass

Each group receives its own preprocessing before combining them into one dataset.

---

# ❓ Why Do We Use ColumnTransformer?

Different types of data require different preprocessing.

For example:

### Numerical Data
Needs:
- Missing value handling
- Feature scaling

### Categorical Data
Needs:
- Missing value handling
- Encoding

Without ColumnTransformer, preprocessing becomes lengthy and difficult to manage.

ColumnTransformer simplifies this process and reduces coding effort.

---

# ⚙️ Preprocessing Steps

## 1. Load Dataset

Read the Titanic dataset using Pandas.

---

## 2. Select Required Features

Features:
- Pclass
- Sex
- Age
- Fare
- Embarked

Target:
- Survived

---

## 3. Split Dataset

Split the data into

- Training Data
- Testing Data

using train_test_split().

---

## 4. Numerical Pipeline

Numerical columns:

- Age
- Fare

Operations performed:

✔ Missing values → Median

✔ Feature Scaling → StandardScaler

---

## 5. Categorical Pipeline

Categorical columns:

- Sex
- Embarked
- Pclass

Operations performed:

✔ Missing values → Most Frequent

✔ One Hot Encoding

---

## 6. ColumnTransformer

Combines

Numerical Pipeline

and

Categorical Pipeline

into one preprocessing step.

---

## 7. Machine Learning Pipeline

The complete pipeline contains:

ColumnTransformer

↓

Logistic Regression

This ensures preprocessing happens automatically before model training.

---

## 8. Model Training

Train the model using

model.fit()

---

## 9. Prediction

Predict survival on test data.

---

## 10. Model Evaluation

Evaluate performance using

Accuracy Score

---

# 📊 Workflow

Dataset

↓

Train-Test Split

↓

ColumnTransformer

├── Numerical Pipeline

│ ├── Median Imputation

│ └── Standard Scaling

│

└── Categorical Pipeline

├── Most Frequent Imputation

└── One Hot Encoding

↓

Processed Dataset

↓

Logistic Regression

↓

Prediction

↓

Accuracy

---

# 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn

---

# 📦 Libraries Used

- pandas
- numpy
- train_test_split
- ColumnTransformer
- Pipeline
- SimpleImputer
- StandardScaler
- OneHotEncoder
- LogisticRegression
- accuracy_score

---

# 🚀 Advantages of ColumnTransformer

- Handles numerical and categorical columns together
- Reduces preprocessing code
- Easy to maintain
- Prevents preprocessing mistakes
- Integrates smoothly with Pipeline
- Improves code readability
- Useful for production-ready machine learning workflows

---

# 📈 Output

The model predicts whether a passenger survived based on the given features after automatic preprocessing using ColumnTransformer.

---

# 🎓 Learning Outcomes

After completing this project, you will understand:

- What ColumnTransformer is
- Why ColumnTransformer is important
- How to preprocess mixed data types
- How to build separate preprocessing pipelines
- How to combine pipelines using ColumnTransformer
- How to integrate preprocessing with a Machine Learning model
- How to train and evaluate a Logistic Regression model

---

# 📖 Conclusion

ColumnTransformer is one of the most important preprocessing tools in Scikit-learn. It allows different transformations to be applied to different feature types in a clean, efficient, and scalable way.

It is widely used in real-world machine learning projects because it simplifies preprocessing and makes pipelines easier to maintain and deploy.
