# 📈 Polynomial Regression Project

This project demonstrates how to implement **Polynomial Regression** using **Scikit-learn** to model and analyze a nonlinear (quadratic) relationship between variables.

## 🔧 Project Overview

The objective of this project is to:
- Understand how polynomial regression can outperform linear regression on non-linear data.
- Visualize the fit of both models.
- Evaluate model accuracy using R² (coefficient of determination).

---

## 🗂️ Project Structure

1. **Data Generation**  
   Synthetic data is generated with a quadratic relationship using NumPy.

2. **Data Visualization**  
   The dataset is visualized using `matplotlib.pyplot` to understand the data trend.

3. **Model Training**  
   - **Linear Regression**
   - **Polynomial Regression** (degree 2)

4. **Model Evaluation**  
   R² score is calculated for both models to compare performance.

5. **Visualization of Results**  
   Best-fit lines for both models are plotted to visualize how well they fit the data.

---

## 🛠️ Technologies and Libraries Used

| Library       | Purpose                        |
|---------------|--------------------------------|
| `numpy`       | Data generation & math ops     |
| `matplotlib`  | Data visualization             |
| `sklearn`     | Model training, transformation, and evaluation |

---

## 📌 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/polynomial-regression-project.git
   cd polynomial-regression-project
