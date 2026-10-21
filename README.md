# Feature Scaling – Phishing URL Detection

## 📌 Project Overview

This project focuses on detecting phishing URLs using Machine Learning. It uses a Decision Tree Classifier to classify URLs as **Phishing** or **Legitimate** based on numerical features from the PhiUSIIL Phishing URL Dataset.

The project demonstrates data preprocessing, feature selection, model training, prediction, and performance evaluation using Python.

## 🎯 Objectives

- Analyze the phishing URL dataset.
- Handle missing values and invalid numerical values.
- Prepare numerical features for machine learning.
- Train a Decision Tree classification model.
- Visualize the decision tree and confusion matrix.
- Evaluate the model using classification metrics

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## 📂 Project Structure

```text
Feature-Scaling/
│
├── Feature_Scaling.ipynb
├── PhiUSIIL_Phishing_URL_Dataset.csv
└── README.md
```

## 📊 Dataset

The project uses the **PhiUSIIL Phishing URL Dataset**.

The dataset is loaded from a CSV file and analyzed to check its shape, column names, missing values, and target label distribution.

**Target labels:**
- `0` – Phishing in the original dataset
- `1` – Legitimate in the original dataset

For model training, the labels are converted to:
- `0` – Legitimate
- `1` – Phishing

Only numerical features are selected for training.

## ⚙️ Project Workflow

1. **Import Libraries** – Load the required Python libraries.
2. **Load Dataset** – Read the CSV file and inspect the data.
3. **Data Preprocessing** – Remove rows with missing target labels, replace infinite values, and fill missing numerical feature values with their column medians.
4. **Feature Selection** – Select numerical columns and exclude the target label.
5. **Train-Test Split** – Split the dataset into 80% training data and 20% testing data.
6. **Model Training** – Train a Decision Tree Classifier with a maximum depth of 5 and balanced class weights.
7. **Visualization** – Display the trained decision tree.
8. **Prediction** – Predict phishing and legitimate labels for the test dataset.
9. **Evaluation** – Calculate accuracy, precision, recall, and the confusion matrix.

## 🤖 Machine Learning Model

The project uses a **Decision Tree Classifier** from Scikit-learn.

Model configuration:
- Maximum depth: `5`
- Class weight: `balanced`
- Random state: `42`

## 📈 Evaluation Metrics

The model is evaluated using the following metrics:

- **Accuracy:** Measures the proportion of correct predictions.
- **Precision:** Measures how many predicted phishing cases are actually phishing.
- **Recall:** Measures how many actual phishing cases are correctly identified.
- **Confusion Matrix:** Shows the counts of correct and incorrect classifications.

The notebook prints the evaluation results and visualizes the confusion matrix.

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Install the required libraries

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
```

### 3. Add the dataset

Place `PhiUSIIL_Phishing_URL_Dataset.csv` in the same directory as the notebook.

### 4. Open Jupyter Notebook

```bash
jupyter notebook
```

Open `Feature_Scaling.ipynb` and run the cells in order.

## 💡 Key Learning Outcomes

- Understanding data preprocessing for machine learning.
- Handling missing and infinite numerical values.
- Selecting features for classification.
- Training and testing a Decision Tree model.
- Visualizing machine learning models.
- Evaluating classification performance.

## 🔮 Future Improvements

- Compare Decision Tree performance with Random Forest and other classifiers
