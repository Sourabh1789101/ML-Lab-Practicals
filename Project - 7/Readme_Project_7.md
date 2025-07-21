# 📧 Spam Detection using Sklearn Pipeline

This project demonstrates how to build a machine learning model to detect spam messages using the `scikit-learn` pipeline. It emphasizes clean, modular design using pipelines for text preprocessing and classification.

---

## 📁 Dataset

The dataset used is a spam classification dataset containing labeled text messages.

- `label`: Identifies whether a message is "spam" or "ham" (non-spam).
- `text`: The actual SMS content.

Sample loading:
```python
import pandas as pd
df = pd.read_csv("spam.csv")
df.head()
```

---

## 🛠️ Tools & Libraries

- **Python**
- **Pandas** – Data manipulation
- **Scikit-learn** – ML modeling and pipeline
- **TfidfVectorizer** – Text feature extraction
- **Train-test split**
- **Naive Bayes** (or other models like Logistic Regression)

---

## 🚀 Project Workflow

1. **Loading the Data**
   - CSV loaded using `pandas.read_csv()`
   - Inspected using `.head()` and `.info()`

2. **Data Preprocessing**
   - Dropping unnecessary columns
   - Label encoding: converting "spam" and "ham" into numerical labels
   - Checking for nulls or imbalanced classes

3. **Splitting the Dataset**
   - Using `train_test_split` to divide the dataset for training and evaluation

4. **Building the ML Pipeline**
   - Vectorizing the SMS text using `TfidfVectorizer`
   - Choosing a model like `MultinomialNB` for classification
   - Combining steps using `Pipeline` from `sklearn`

Example:
```python
from sklearn.pipeline import Pipeline
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.naive_bayes import MultinomialNB

pipeline = Pipeline([
    ('tfidf', TfidfVectorizer()),
    ('model', MultinomialNB())
])
```

5. **Model Training and Evaluation**
   - Fitting the pipeline with training data
   - Making predictions on test data
   - Evaluating using:
     - `accuracy_score`
     - `confusion_matrix`
     - `classification_report`

---

## ✅ Results

- Model successfully classifies spam vs. ham messages
- Achieved high accuracy and precision
- Clean modular code using `Pipeline`

---

## 📈 Future Enhancements

- Try other models like:
  - Logistic Regression
  - Random Forest
  - SVM
- Use hyperparameter tuning (`GridSearchCV`)
- Visualize results using confusion matrix heatmap
- Deploy model using Flask/Streamlit as a web app

---

## 📄 License

This project is for educational purposes only.
