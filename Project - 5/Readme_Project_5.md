# 🌸 Iris Dataset Analysis

This project presents a basic **Exploratory Data Analysis (EDA)** of the well-known **Iris dataset** using Python's data science libraries.

The Iris dataset is a classic and very easy multi-class classification dataset that contains measurements of iris flowers from three different species.

---

## 📌 Objective

- Load and explore the Iris dataset
- Identify unique classes in the target feature (`species`)
- Check for null/missing values
- Visualize feature relationships using pair plots

---

## 🛠️ Libraries Used

| Library      | Purpose                          |
|--------------|----------------------------------|
| `seaborn`    | Data visualization (e.g., pairplots) |
| `pandas`     | Data manipulation and inspection |
| `numpy`      | Numerical computations (if needed) |

---

## 📁 Project Components

1. **Data Loading**
   - The dataset is loaded using:
     ```python
     df = sns.load_dataset('iris')
     ```
   - Displays the first few rows using `df.head()`.

2. **Data Exploration**
   - Identifies unique species:
     ```python
     df['species'].unique()
     ```
   - Checks for missing/null values:
     ```python
     df.isnull().sum()
     ```

3. **Exploratory Data Analysis**
   - A **pairplot** is created using:
     ```python
     sns.pairplot(df, hue='species')
     ```
   - This visualizes the relationships among features and how they differ across species.

---

## 🔍 Insights

- The dataset includes 3 species: *setosa*, *versicolor*, and *virginica*.
- There are no missing values in the dataset.
- Clear separation can be observed between *setosa* and other species in the pair plots.
- Features like **petal length** and **petal width** are good indicators for classification.

---

## ▶️ How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/iris-data-analysis.git
   cd iris-data-analysis
