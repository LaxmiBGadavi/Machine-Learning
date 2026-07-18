# 📊 Logistic Regression

> A complete implementation of **Logistic Regression** using Python and Scikit-learn for solving classification problems.

 

# 📖 Introduction

Logistic Regression is one of the most fundamental **Supervised Machine Learning** algorithms used for **classification problems**.

Despite its name containing the word **Regression**, it is **not used for predicting continuous values**. Instead, it predicts **categorical outcomes** by estimating the probability that an input belongs to a particular class.

Examples include:

- Disease Prediction
- Spam Detection
- Customer Churn Prediction
- Loan Approval
- Fraud Detection

---

# 🧠 What is Logistic Regression?

Logistic Regression is a statistical algorithm that predicts the probability of a data point belonging to a specific class.

Instead of predicting a numerical value like Linear Regression, Logistic Regression predicts:

- Yes / No
- True / False
- 0 / 1
- Positive / Negative

The output is always a probability between **0 and 1**.

---

# ❓ Why Logistic Regression?

Logistic Regression is preferred because it:

- Simple and easy to understand
- Fast training
- Efficient for binary classification
- Produces probability scores
- Easy to interpret
- Works well on linearly separable datasets

---

# 📌 When to Use Logistic Regression?

Use Logistic Regression when:

✅ Target variable is categorical

Examples:

- Pass / Fail
- Spam / Not Spam
- Disease / Healthy
- Fraud / Genuine
- Loan Approved / Rejected

---

# 📊 Classification vs Regression

| Regression | Classification |
|------------|---------------|
| Predicts Continuous Values | Predicts Categories |
| Output is Numeric | Output is Class Label |
| Example: House Price | Example: Spam Detection |

---

# 🔢 Types of Logistic Regression

## 1. Binary Logistic Regression

Predicts one of two classes.

Example:

- Yes / No
- Pass / Fail

---

## 2. Multinomial Logistic Regression

Used when there are more than two classes.

Example:

- Red
- Green
- Blue

---

## 3. Ordinal Logistic Regression

Used when classes have an order.

Example:

- Low
- Medium
- High

---

# ⚙️ How Logistic Regression Works

The algorithm follows these steps:

1. Collect Dataset
2. Clean Dataset
3. Encode Categorical Data
4. Split Dataset
5. Train Logistic Regression
6. Predict Probability
7. Convert Probability into Class
8. Evaluate Performance

---

# 📈 Sigmoid Function

Unlike Linear Regression, Logistic Regression uses the **Sigmoid Function**.

The sigmoid function converts any real value into a probability between **0 and 1**.

- If Probability ≥ 0.5 → Class 1
- If Probability < 0.5 → Class 0

The sigmoid curve has an S-shape.

---

# 📌 Assumptions

Logistic Regression assumes:

- Independent observations
- Little or no multicollinearity
- Linear relationship between features and log odds
- Large sample size
- No extreme outliers

---

# 🔄 Machine Learning Workflow

```
Dataset

↓

Data Cleaning

↓

Encoding

↓

Feature Scaling

↓

Train-Test Split

↓

Model Training

↓

Prediction

↓

Evaluation

↓

Deployment
```

---

# 📂 Dataset

The dataset contains:

- Independent Features (X)
- Target Variable (Y)

Example:

```
Age | Salary | Purchased
```

Where:

- Age
- Salary

are input features.

Purchased is the target variable.

---

# 🧹 Data Preprocessing

Before training:

- Handle Missing Values
- Remove Duplicates
- Encode Categorical Variables
- Feature Scaling
- Separate Features and Target

---

# ⚖️ Feature Scaling

Feature Scaling improves model performance by bringing all features to the same scale.

Common methods:

- StandardScaler
- MinMaxScaler

---

# ✂️ Train-Test Split

The dataset is divided into:

- 80% Training Data
- 20% Testing Data

Training Data:

Used to train the model.

Testing Data:

Used to evaluate the model.

---

# 🤖 Model Training

Scikit-learn provides:

```python
from sklearn.linear_model import LogisticRegression

model = LogisticRegression()

model.fit(X_train, y_train)
```

The model learns the relationship between features and target labels.

---

# 🔮 Prediction

Predictions are made using:

```python
y_pred = model.predict(X_test)
```

The model predicts:

- Class Labels
- Probability Scores

---

# 📊 Model Evaluation

## Accuracy

Measures overall correctness.

Higher accuracy means better predictions.

---

## Confusion Matrix

A confusion matrix shows:

- True Positive (TP)
- True Negative (TN)
- False Positive (FP)
- False Negative (FN)

It helps understand classification performance.

---

## Precision

Precision answers:

Out of all predicted positives,

how many were actually positive?

Higher precision means fewer False Positives.

---

## Recall

Recall answers:

Out of all actual positives,

how many were correctly predicted?

Higher recall means fewer False Negatives.

---

## F1 Score

F1 Score balances:

- Precision
- Recall

Useful for imbalanced datasets.

---

## ROC Curve

ROC Curve compares:

- True Positive Rate
- False Positive Rate

A better model has a curve closer to the top-left corner.

---

## AUC Score

AUC stands for:

Area Under ROC Curve

Higher AUC indicates a better classifier.

---

# ✅ Advantages

- Easy to implement
- Fast training
- Efficient
- Interpretable
- Produces probabilities
- Works well for binary classification
- Less computational cost

---

# ❌ Limitations

- Cannot capture complex relationships
- Sensitive to outliers
- Requires feature engineering
- Works best with linear decision boundaries

---

# 🌍 Real-World Applications

Logistic Regression is used in:

- Disease Prediction
- Email Spam Detection
- Credit Card Fraud Detection
- Customer Churn Prediction
- Loan Approval Prediction
- Marketing Campaign Analysis
- Employee Attrition Prediction
- Sentiment Analysis

---

# 📂 Repository Structure

```
Logistic_Regression/

│── Logistic_Regression.ipynb

│── Dataset.csv

│── README.md

│── requirements.txt

│── images/
```

---

# 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

# ▶️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Logistic_Regression.git
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run Jupyter Notebook:

```bash
jupyter notebook
```

---

# 🚀 How to Run

1. Open Jupyter Notebook

2. Load Dataset

3. Run each cell

4. Train Logistic Regression

5. Predict Results

6. Evaluate Model

---

# 🎯 Learning Outcomes

After completing this project, I learned:

- Supervised Machine Learning
- Classification Problems
- Logistic Regression
- Sigmoid Function
- Data Cleaning
- Feature Encoding
- Feature Scaling
- Train-Test Split
- Model Training
- Prediction
- Accuracy
- Confusion Matrix
- Precision
- Recall
- F1 Score
- ROC-AUC

---

# 📚 Future Improvements

- Hyperparameter Tuning
- Cross Validation
- Feature Selection
- Grid Search CV
- Compare with Random Forest
- Compare with SVM
- Compare with Decision Tree

---

# 👩‍💻 Author

**Laxmi Gadavi**

🎓 B.E. Artificial Intelligence & Data Science

💻 Passionate about Machine Learning, Data Science, and Artificial Intelligence.

⭐ If you found this project helpful, consider giving it a **Star** on GitHub!
