
# Spam Detection using Sklearn Pipeline

This project demonstrates how to build a machine learning model to detect spam messages using the `scikit-learn` pipeline. The approach focuses on clean, modular design using pipelines for preprocessing and classification.

## 📂 Dataset

The dataset used in this project is a spam classification dataset (`spam.csv`) containing labeled text messages.

- `label`: Indicates whether a message is "spam" or "ham" (not spam).
- `text`: The actual message content.

## ⚙️ Tools & Libraries

- Python
- Pandas
- Scikit-learn (Sklearn)
- TfidfVectorizer
- Train-Test Split
- Naive Bayes / Logistic Regression / Random Forest (assumed models)

## 📌 Project Workflow

1. **Data Loading**  
   The dataset is loaded using Pandas:
   ```python
   import pandas as pd
   df = pd.read_csv("spam.csv")
   ```

2. **Preprocessing**  
   Basic cleaning and renaming of columns, and label encoding of `spam` and `ham`.

3. **Train-Test Split**  
   The data is split into training and testing sets for evaluation purposes.

4. **Pipeline Construction**  
   A `Pipeline` is created using:
   - `TfidfVectorizer` for converting text to numeric form
   - A classifier like `MultinomialNB` or `LogisticRegression` for prediction

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

5. **Model Training & Evaluation**  
   The pipeline is trained and tested to evaluate its accuracy using:
   - `accuracy_score`
   - `classification_report`
   - `confusion_matrix`

## ✅ Results

- Achieved high accuracy for spam classification (specific numbers shown in the notebook).
- Pipeline approach makes the model reusable and easy to test with different algorithms.

## 📈 Future Work

- Try more classifiers (e.g., SVM, Random Forest).
- Tune hyperparameters using GridSearchCV.
- Deploy the model as a web app using Flask or Streamlit.

## 📎 License

This project is for educational purposes.
