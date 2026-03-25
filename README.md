# Machine-Learning-Tutorial-Individual-Assignment
An example of the Vanishing Gradient issue in Deep Neural Networks using PyTorch. uses a unique dataset for predicting athlete injuries to compare Sigmoid and ReLU activation functions.

This repository contains an educational PyTorch tutorial demonstrating the **Vanishing Gradient Problem** in Deep Multilayer Perceptrons (MLPs). It provides a side-by-side mathematical and visual comparison of the **Sigmoid** and **ReLU** activation functions.

To make the concepts practical, the tutorial applies these networks to a simulated sports analytics dataset to predict athlete injury risks based on biological and training metrics.

## 🎯 Project Objective
The goal of this project is to visually prove *why* deep networks fail when using traditional activation functions (like Sigmoid) due to the chain rule of calculus shrinking the gradient during backpropagation, and *how* the Rectified Linear Unit (ReLU) solves this mathematical trap.

## 🗂️ Repository Contents
* **`Tutorial_Code.ipynb`**: The complete Jupyter/Colab notebook containing the data generation, preprocessing, PyTorch model architectures, custom training loops, and visualization code.
* **`Machine_Learning_Tutorial.pdf`**: The full written tutorial explaining the theory, mathematics, and results of the experiment.
* **`athlete_injury_data.csv`**: A custom dataset containing 500 records of athlete biometrics (e.g., sprint speed, sleep hours, training load) and a binary injury risk target.
* **`imageOutput.png`**: The generated 2x2 visual dashboard showing gradient flow, loss curves, confusion matrices, and ROC-AUC curves.

## 📊 The Dataset
The dataset (`athlete_injury_data.csv`) is generated programmatically within the notebook. It contains 11 continuous and categorical features representing athlete biometrics. The target variable, `Injury_Risk`, is a highly non-linear combination of training load, sleep deprivation, and muscle asymmetry.

## 🚀 How to Run the Code

### Option 1: Google Colab (Recommended)
1. Upload the `Tutorial_Code.ipynb` file to Google Colab.
2. Run all cells. The notebook will automatically generate the dataset, train the models, and output the visual dashboard.

### Option 2: Local Python Environment
1. Clone this repository.
