# Comparative Analysis of Machine Learning Models for Obesity Level Prediction

## Overview

This project explores and compares different machine learning classification algorithms to predict an individual's obesity level based on physical characteristics and lifestyle-related factors.

The project focuses on evaluating **Decision Tree, Random Forest, and Support Vector Machine (SVM)** models to understand their performance on an obesity classification task.

The repository includes Jupyter notebooks for model development, a dataset, a saved Random Forest model, a Streamlit-based prediction interface, and project documentation.

## Objectives

- Analyze the factors associated with different obesity levels.
- Prepare and preprocess the dataset for machine learning.
- Implement Decision Tree, Random Forest, and SVM classification models.
- Compare model performance using appropriate evaluation metrics.
- Save a trained model for future predictions.
- Develop an interactive interface for obesity level prediction.

## Dataset

The project uses `ObesityDataSet.csv`, which contains information about individuals' physical characteristics, eating habits, physical activity, and lifestyle.

The target variable, `NObeyesdad`, represents the obesity classification.

The dataset includes seven possible categories:

1. Insufficient Weight
2. Normal Weight
3. Overweight Level I
4. Overweight Level II
5. Obesity Type I
6. Obesity Type II
7. Obesity Type III

The dataset supports a multiclass classification task in which the model predicts one of these categories from the input features.

## Machine Learning Models

### 1. Decision Tree Classifier

A Decision Tree learns decision rules from the input features and uses them to classify individuals into obesity categories. It is useful for understanding how feature-based decisions can be made.

### 2. Random Forest Classifier

Random Forest combines multiple decision trees to produce a classification prediction. It can improve generalization compared with an individual tree and is used as the trained model in the prediction interface included in this repository.

### 3. Support Vector Machine (SVM)

SVM identifies decision boundaries that separate different classes. It is included to compare a margin-based classification approach with the tree-based models.

##  Technologies Used

- **Python** — programming language
- **Pandas** — data manipulation and analysis
- **NumPy** — numerical computation
- **Scikit-learn** — machine learning and preprocessing
- **Matplotlib / Seaborn** — data visualization, where used
- **Jupyter Notebook** — experimentation and model evaluation
- **Streamlit** — interactive prediction interface
- **Pickle** — serialization of the trained model and scaler

##  Repository Structure

```text
Comparative-Analysis-of-Machine-Learning-Models-for-Obesity-Level-Prediction/
│
├── ObesityDataSet.csv
├── decisiontree.ipynb
├── randomforest.ipynb
├── svm.ipynb
├── randomforest.pickle
├── randomforestUI.py
├── CpmparativeAnalysisDocumentation.pdf
└── README.md
```

### File Description

| File | Description |
|---|---|
| `ObesityDataSet.csv` | Dataset used for model development |
| `decisiontree.ipynb` | Decision Tree implementation and analysis |
| `randomforest.ipynb` | Random Forest implementation and analysis |
| `svm.ipynb` | SVM implementation and analysis |
| `randomforest.pickle` | Serialized Random Forest model and scaler |
| `randomforestUI.py` | Streamlit application for predictions |
| `CpmparativeAnalysisDocumentation.pdf` | Detailed project documentation |
| `README.md` | Project overview and instructions |

##  Installation and Setup

### Prerequisites

- Python 3.9 or a compatible version
- pip package manager
- Git

### 1. Clone the repository

```bash
git clone https://github.com/Tulsi12/Comparative-Analysis-of-Machine-Learning-Models-for-Obesity-Level-Prediction.git
```

### 2. Navigate to the project directory

```bash
cd Comparative-Analysis-of-Machine-Learning-Models-for-Obesity-Level-Prediction
```

### 3. Create a virtual environment (recommended)

```bash
python -m venv venv
```

Activate it:

**Windows**
```bash
venv\Scripts\activate
```

**Linux / macOS**
```bash
source venv/bin/activate
```

### 4. Install the required libraries

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter streamlit
```

##  Running the Project

### Run the Jupyter notebooks

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open the notebooks to explore the individual model implementations, preprocessing steps, and evaluation results.

### Run the prediction interface

The repository includes a Streamlit interface that loads the saved Random Forest model and its associated scaler.

Run the application from the project directory:

```bash
streamlit run randomforestUI.py
```

Streamlit will provide a local URL in the terminal. Open that URL in your browser to access the application.

Enter the requested physical characteristics and click **Predict** to view the predicted obesity category.

**Note:** The prediction interface uses the saved model and scaler in `randomforest.pickle`. Keep this file in the project directory when running the application.

## Model Evaluation

The models are intended to be compared using suitable classification metrics, including:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrix

These metrics help evaluate overall classification performance and how effectively each model distinguishes between obesity categories.

For the actual performance values and final comparison, refer to the results in the notebooks and the project documentation.

##  Project Workflow

1. Load and inspect the obesity dataset.
2. Explore the dataset and its features.
3. Preprocess the data and prepare the target labels.
4. Train the Decision Tree, Random Forest, and SVM classifiers.
5. Evaluate and compare the models.
6. Save the trained Random Forest model and scaler.
7. Use the Streamlit interface to generate predictions.

## ⚠️ Disclaimer

This project is intended for educational and research purposes. Its predictions are based on patterns in the dataset and should not be treated as a medical diagnosis or a substitute for professional healthcare advice.

##  Documentation

For a more detailed explanation of the methodology, implementation, and findings, see [CpmparativeAnalysisDocumentation.pdf](CpmparativeAnalysisDocumentation.pdf).

