# 🌳 Decision Tree Classifier from Scratch (Information Gain & Entropy)

This project demonstrates how to build a **Decision Tree Classifier from scratch** using core concepts of **Entropy** and **Information Gain** — fundamental to Machine Learning.

Unlike typical models built using libraries like `scikit-learn`, this notebook manually constructs a decision tree using custom Python functions and visualizes it using `Graphviz`.

---

## 🧠 Key Concepts Used

### 📘 Entropy
Entropy measures the randomness in the data. A lower entropy indicates better classification.

### 📘 Information Gain
Information Gain measures the reduction in entropy achieved by splitting the dataset on a particular attribute.

---

## 🛠️ Technologies Used

- Python
- Pandas – for data manipulation
- Math – for entropy/log calculations
- Graphviz – for visualizing the tree
- Jupyter Notebook

---

## 🗃️ Dataset Used

The dataset is a small, manually created DataFrame representing customer decisions about purchasing a computer, with features like:

| Age         | Income | Student | Buy Computer |
|-------------|--------|---------|--------------|
| Young       | High   | Yes     | Yes          |
| Young       | High   | No      | No           |
| Middle-aged | Low    | No      | Yes          |
| Old         | Medium | Yes     | No           |
| Old         | High   | Yes     | Yes          |
| Old         | Low    | No      | No           |

---

## 🚀 How It Works

1. **Calculate Entropy** of the dataset.
2. **Compute Information Gain** for each attribute.
3. **Select the best attribute** (with highest gain) for splitting.
4. **Recursively split** subsets until:
   - All records belong to a single class.
   - No attributes are left.
5. **Render Tree** using Graphviz.

---

## 📈 Output

The final output is a **visual decision tree** saved as a PNG image:

```
Root
 ├── Age = Young
 │    └── ...
 ├── Age = Old
 │    └── ...
 └── Age = Middle-aged
      └── ...
```

You can view the tree image generated as `decision_tree.png`.

---

## 📦 How to Run This Project

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/decision-tree-from-scratch.git
   cd decision-tree-from-scratch
   ```

2. Install dependencies:
   ```bash
   pip install pandas graphviz
   ```

3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook "Project - 9.ipynb"
   ```

4. Make sure Graphviz is installed in your system. On Windows, you can download it from:  
   👉 https://graphviz.gitlab.io/_pages/Download/Download_windows.html

---

## 🙋‍♂️ Why This Project?

This project helps you:
- Understand how decision trees **actually work under the hood**.
- Get familiar with **Entropy**, **Information Gain**, and **recursion**.
- Visualize models using **Graphviz**, which is a widely used tool for decision trees.

---

## 🧾 License

This project is licensed under the **MIT License** – use it freely!

---

## 🤝 Contributions Welcome

If you'd like to extend the tree builder or test it on a larger dataset, feel free to contribute!
