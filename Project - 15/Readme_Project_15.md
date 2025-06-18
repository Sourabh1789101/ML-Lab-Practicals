# 🏡 Boston Housing Price Prediction using ANN

This project showcases the implementation of an Artificial Neural Network (ANN) for solving a regression problem using the Boston Housing dataset. The model is built using TensorFlow and Keras.

## 📦 Dataset

- **Source**: `tensorflow.keras.datasets.boston_housing`
- **Features**: 13 numerical attributes (e.g., crime rate, number of rooms, tax rate, etc.)
- **Target**: Median value of owner-occupied homes in $1000s.

## 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- NumPy

## 🧪 Model Architecture

### Model 1
- Input Layer: 13 neurons
- Output Layer: 1 neuron (linear activation)
- Loss Function: `msle` (Mean Squared Logarithmic Error)
- Optimizer: `SGD`
- Metrics: `accuracy`, `msle`

### Model 2 (Extended)
- Hidden Layers: Includes Dense layers with 50+ units (details in notebook)
- Activation Functions: `relu`, `linear`
- Trained over multiple epochs for improved accuracy

## 📊 Training & Evaluation

- The model is trained on the training set (`x_train`, `y_train`) and evaluated on the test set (`x_test`, `y_test`).
- Evaluation metrics and loss are displayed to gauge model performance.

## 📁 Files

- `Project - 15.ipynb`: Main notebook containing all implementation steps.

## 🚀 Getting Started

To run the notebook:

```bash
pip install tensorflow
