# 🔤 Encoding Techniques in Machine Learning

This repository demonstrates different encoding techniques used in Machine Learning to convert categorical data into numerical values. Encoding is an essential data preprocessing step because most machine learning algorithms cannot work directly with text data.

---

## 📖 What is Encoding?

Encoding is the process of transforming categorical (text) data into numerical values so that machine learning algorithms can understand and process it.

### Why do we use Encoding?

Machine Learning models work with numbers, not text.

Example:

Before Encoding

| Gender |
|---------|
| Male |
| Female |
| Male |

After Encoding

| Gender |
|---------|
| 1 |
| 0 |
| 1 |

---

# 📚 Types of Encoding

## 1️⃣ Label Encoding

### Description
Assigns a unique integer to each category.

### Example

| Color |
|--------|
| Red |
| Green |
| Blue |

Encoded

Red → 2

Green → 1

Blue → 0

### When to Use

- Binary categories
- Target variable
- Ordinal data

### Advantages

- Simple
- Fast
- Less memory

### Disadvantages

Creates an artificial order for nominal data.

---

## 2️⃣ One-Hot Encoding

### Description

Creates separate columns for each category.

### Example

| Color |
|--------|
| Red |
| Blue |
| Green |

Encoded

| Red | Blue | Green |
|------|------|-------|
|1|0|0|
|0|1|0|
|0|0|1|

### When to Use

- Nominal data
- Categories without order

Examples

- Gender
- City
- Department

### Advantages

- No false ordering
- Most commonly used

### Disadvantages

Creates many columns when categories are large.

---

## 3️⃣ Ordinal Encoding

### Description

Assigns numbers according to category order.

### Example

Low → 0

Medium → 1

High → 2

Very High → 3

### When to Use

Ordered categorical data.

Examples

- Education Level
- Customer Rating
- Shirt Size

### Advantages

Maintains ranking information.

### Disadvantages

Should not be used for unordered categories.

---

## 4️⃣ Binary Encoding

### Description

Converts Label Encoding values into binary numbers.

Example

A → 000

B → 001

C → 010

D → 011

### When to Use

High-cardinality categorical features.

Examples

- Product IDs
- Customer IDs

### Advantages

- Uses fewer columns than One-Hot Encoding
- Efficient

### Disadvantages

Slightly difficult to interpret.

---

## 5️⃣ Frequency Encoding

### Description

Replaces each category with its occurrence count.

### Example

City

Delhi

Mumbai

Delhi

Pune

Delhi

Encoded

Delhi → 3

Mumbai → 1

Pune → 1

### When to Use

Large number of unique categories.

### Advantages

- Simple
- No extra columns

### Disadvantages

Different categories with the same frequency receive the same value.

---

## 6️⃣ Target Encoding

### Description

Replaces categories with the average value of the target variable.

### Example

| City | Purchased |
|------|-----------|
|Delhi|1|
|Delhi|0|
|Mumbai|1|

Encoded

Delhi → 0.5

Mumbai → 1.0

### When to Use

Large datasets with many categories.

### Advantages

Improves model performance.

### Disadvantages

May cause data leakage if not used correctly.

---

# 📊 Comparison

| Encoding | Best For | Preserves Order | Creates Extra Columns |
|----------|----------|-----------------|------------------------|
| Label Encoding | Binary / Target | ✅ Yes | ❌ No |
| One-Hot Encoding | Nominal Data | ❌ No | ✅ Yes |
| Ordinal Encoding | Ordered Data | ✅ Yes | ❌ No |
| Binary Encoding | High Cardinality | ❌ No | Few |
| Frequency Encoding | High Cardinality | ❌ No | ❌ No |
| Target Encoding | Large Datasets | Depends | ❌ No |

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook

---

# 📂 Repository Structure

```
Encoding-Techniques/
│
├── Encoding_Practical.ipynb
├── dataset.csv
├── README.md
```

---

# ▶️ How to Run

1. Clone this repository

```bash
git clone https://github.com/yourusername/Encoding-Techniques.git
```

2. Install required libraries

```bash
pip install pandas numpy scikit-learn
```

3. Open Jupyter Notebook

```bash
jupyter notebook
```

4. Run all notebook cells.

---

# 🎯 Learning Outcomes

- Understand why encoding is important.
- Learn different encoding techniques.
- Know when to use each encoding method.
- Apply encoding using Scikit-learn.
- Prepare categorical data for Machine Learning models.

---

# 👩‍💻 Author

**Laxmi Gadavi**

Artificial Intelligence & Data Science Graduate

---
