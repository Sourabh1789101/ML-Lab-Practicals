
# 📊 Startup Profit Prediction - Multiple Linear Regression

This project aims to predict the profit of 50 startups using Multiple Linear Regression. It is built using Python and key data science libraries like `pandas`, `numpy`, `matplotlib`, and `scikit-learn`.

---

## 📁 Dataset Used

**File:** `50_Startups.csv`

**Columns:**
- `R&D Spend`: Money spent on research and development
- `Administration`: Money spent on administration
- `Marketing Spend`: Money spent on marketing
- `State`: The state where the startup is located
- `Profit`: The target variable we aim to predict

---

## 🧪 Steps Performed

1. **Import Libraries**
   ```python
   import numpy as np
   import matplotlib.pyplot as plt
   import pandas as pd
   ```

2. **Load Dataset**
   ```python
   df = pd.read_csv('50_Startups.csv')
   df.head()
   ```

3. **Data Preprocessing**
   - Handle categorical variable (`State`)
   - Split features and target
   - Apply one-hot encoding

4. **Model Building**
   - Use `LinearRegression()` from `sklearn.linear_model`
   - Fit the model to training data

5. **Prediction**
   - Evaluate the model using R² Score or Mean Squared Error

6. **Visualization**
   - Optional: Plot predicted vs actual values

---

## ⚙️ Technologies Used

- Python 3
- NumPy
- Pandas
- Matplotlib
- scikit-learn

---

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/project-startup-profit.git
   cd project-startup-profit
   ```

2. Install dependencies:
   ```bash
   pip install numpy pandas matplotlib scikit-learn
   ```

3. Run the notebook:
   ```bash
   jupyter notebook Project\ -\ 4.ipynb
   ```

---

## 📈 Sample Output

> Visualizations and model accuracy results go here (can add after running all cells).

---

## 💡 Future Improvements

- Add markdown explanations in the notebook
- Implement feature selection techniques
- Try other models like Ridge or Lasso Regression

---

## 📬 Contact

**Sourabh Kumar**  
📧 [sourabhkumar99174@gmail.com](mailto:sourabhkumar99174@gmail.com)  
🌐 [LinkedIn](https://www.linkedin.com/in/sourabh-kumar-271099318) | [GitHub](https://github.com/Sourabh1789101)
