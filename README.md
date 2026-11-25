# Breast-cancer-prediction-

# 🎗️ Breast Cancer Prediction Using Machine Learning

## 📌 Project Overview

This project focuses on building a **Machine Learning-based Breast Cancer Prediction System** that classifies breast cancer tumors into two categories:

- 🟢 **Benign:** Non-cancerous tumor.
- 🔴 **Malignant:** Cancerous tumor.

The main objective is to explore and compare different Machine Learning classification algorithms and identify the best-performing model based on evaluation metrics.

Three Machine Learning algorithms are implemented and compared to determine their predictive performance.

## 🎯 Project Objectives

- Understand and analyze the Breast Cancer Wisconsin dataset.
- Perform data preprocessing and exploratory data analysis.
- Train multiple Machine Learning classification models.
- Compare model performance using evaluation metrics.
- Apply 5-Fold Cross Validation.
- Analyze model predictions using a Confusion Matrix.
- Identify important features influencing predictions.

## 📊 Dataset Information

This project uses the **Breast Cancer Wisconsin Diagnostic Dataset** available through Scikit-learn's built-in datasets.

| Dataset Details | Information |
|---|---|
| Total Samples | 569 |
| Total Features | 30 |
| Total Columns (including target and diagnosis) | 32 |
| Benign Cases | 357 |
| Malignant Cases | 212 |
| Missing Values | 0 |
| Duplicate Rows | 0 |

### 🔍 Dataset Features

The dataset contains numerical features describing characteristics of cell nuclei:

- Mean Radius
- Mean Texture
- Mean Perimeter
- Mean Area
- Mean Smoothness
- Mean Compactness
- Mean Concavity
- Mean Concave Points
- Mean Symmetry
- Mean Fractal Dimension

These measurements are available in three groups:

- Mean Features
- Standard Error Features
- Worst Features

## ⚙️ Technologies & Libraries Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| NumPy | Numerical Operations |
| Pandas | Data Manipulation |
| Matplotlib | Data Visualization |
| Scikit-learn | Machine Learning |
| StandardScaler | Feature Scaling |
| Jupyter Notebook | Development Environment |

## 🧠 Machine Learning Algorithms

Three classification algorithms were implemented:

### 1. Logistic Regression
A supervised classification algorithm used to predict whether a tumor is Benign or Malignant.

- StandardScaler for feature scaling.
- Maximum iterations: 1000.

### 2. Random Forest Classifier
An ensemble learning algorithm that combines multiple decision trees to improve prediction performance.

- Number of estimators: 200.
- Random state: 42.

### 3. Decision Tree Classifier
A tree-based classification algorithm that makes predictions using feature-based decision rules.

- Maximum depth: 5.
- Random state: 42.

## 🔄 Project Workflow

1. Import required libraries.
2. Load the Breast Cancer Wisconsin dataset.
3. Convert the dataset into a Pandas DataFrame.
4. Perform initial data exploration.
5. Check missing values and duplicate records.
6. Separate independent features (X) and target variable (y).
7. Split the dataset into training and testing sets.
8. Train three Machine Learning models.
9. Evaluate models using performance metrics.
10. Perform 5-Fold Cross Validation.
11. Identify the best-performing model.
12. Generate Confusion Matrix and Classification Report.
13. Analyze feature importance.
14. Perform sample predictions.

## 📈 Model Performance & Results

The following results were obtained using an 80:20 train-test split.

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| Logistic Regression | **98.25%** | 98.61% | 98.61% | 98.61% |
| Random Forest | 95.61% | 95.89% | 97.22% | 96.55% |
| Decision Tree | 92.11% | 95.65% | 91.67% | 93.62% |

### 🏆 Best Performing Model

**Logistic Regression achieved the highest test accuracy of 98.25%.**

5-Fold Cross Validation Results:

| Model | CV Accuracy |
|---|---:|
| Logistic Regression | 98.07% |
| Random Forest | 95.78% |
| Decision Tree | 91.91% |

## 📉 Confusion Matrix

The Confusion Matrix of the best-performing model (Logistic Regression) produced the following results:

```text
                 Predicted
                 Malignant  Benign

Actual Malignant     41       1
Actual Benign         1      71
```

- True Positives (Benign): 71
- True Negatives (Malignant): 41
- False Positives: 1
- False Negatives: 1

## 🔬 Feature Importance

Random Forest was also used to identify the top 10 important features.

| Feature | Importance |
|---|---:|
| Worst Perimeter | 0.1331 |
| Worst Area | 0.1281 |
| Worst Concave Points | 0.1081 |
| Mean Concave Points | 0.0944 |
| Worst Radius | 0.0906 |
| Mean Radius | 0.0587 |
| Mean Perimeter | 0.0552 |
| Mean Area | 0.0499 |
| Mean Concavity | 0.0462 |
| Worst Concavity | 0.0354 |

## 📊 Visualizations

The project generates:

- 📊 Model Accuracy Comparison
- 🔲 Confusion Matrix
- 📈 Classification Performance Analysis
- 🔬 Random Forest Feature Importance

The notebook saves the evaluation visualization as `results.png`.

## 🚀 How to Run This Project

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Breast-Cancer-Prediction.git
```

### 2. Navigate to the Project Folder

```bash
cd Breast-Cancer-Prediction
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

### 4. Activate the Environment

**Windows PowerShell:**

```powershell
.\venv\Scripts\Activate.ps1
```

### 5. Install Required Libraries

```bash
pip install numpy pandas matplotlib scikit-learn jupyter
```

### 6. Launch Jupyter Notebook

```bash
jupyter notebook
```

### 7. Run the Notebook

Open `Breast cancer prediction.ipynb` and execute the cells sequentially.

## 📁 Project Structure

```text
Breast-Cancer-Prediction/
│
├── Breast cancer prediction.ipynb
├── breast_cancer_data.csv
├── results.png
└── README.md
```

*Note: The CSV file and results image are generated when the corresponding notebook cells are executed.*

## 💡 Key Learnings

Through this project, I gained practical experience in:

- Understanding supervised Machine Learning.
- Working with classification algorithms.
- Data preprocessing and feature scaling.
- Training and testing ML models.
- Evaluating classification performance.
- Understanding Precision, Recall, F1-Score and Accuracy.
- Implementing Cross Validation.
- Analyzing Confusion Matrices.
- Understanding Feature Importance.
- Making predictions using trained ML models.

## ⚠️ Disclaimer

This project is developed for **educational and learning purposes only**.

It is not a clinically validated diagnostic system and must not be used to diagnose breast cancer or make medical decisions. Actual diagnosis requires evaluation by qualified healthcare professionals.

## 👨‍💻 Author

**Dheeraj Chouhan**

Aspiring AI/ML Engineer | Python | Data Science | Machine Learning

- 🐙 GitHub: https://github.com/dheeraj24-coder
- 💼 LinkedIn: https://www.linkedin.com/in/dheeraj-chouhan-7a6996371/

---
  ⭐ If you find this project useful, consider giving it a star!
