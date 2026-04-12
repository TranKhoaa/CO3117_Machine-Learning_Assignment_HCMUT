# CO3117_Machine-Learning_Assignment_HCMUT
## Assignment 1: Machine Learning with Tabular Data

**Course:** CO3117 – Machine Learning - Group 11
**Semester:** 252 – Academic Year 2025–2026  
**Department:** Department of Computer Science, Ho Chi Minh City University of Technology, VNU-HCM  
**Instructor:** PhD. Trương Vĩnh Lân  

---

## Team Members

| Full Name           | Student ID | Email                     |
|---------------------|------------|---------------------------|
| Trần Đăng Khoa      | 2252363    | khoa.tran906@hcmut.edu.vn |
| Phan Trần Quốc Tuấn | 2353273    | email                     |
| Trần Gia Lâm        | 2352670    | email                     |
| Nguyễn Tấn Hưng     | 2352439    | email                     |
| Nguyễn Hữu Cầu      | 2352129    | email                     |

---

## Project Objectives

This project applies the machine learning pipeline to a tabular dataset (Home Value Prediction) with the following objectives:

- Perform thorough **Exploratory Data Analysis (EDA)** to understand data distributions, detect missing values, outliers, and relationships between features.
- Build a **configurable traditional ML pipeline** covering data preprocessing (imputation, encoding, scaling), feature engineering, model training, and evaluation.
- Train and compare multiple classification/regression models: **Logistic Regression**, **Support Vector Machine (SVM)**, and **Random Forest**, across different configurations and hyperparameters.
- Analyze model performance using appropriate metrics (accuracy, precision, recall, F1-score) and draw meaningful conclusions about trade-offs between approaches.
- Implement a **deep learning pipeline** and compare its performance against traditional ML methods.

---

## Project Structure

```
.
├── src/
│   ├── EDA+preprocessing.ipynb     # Exploratory Data Analysis and data preprocessing
│   ├── logistic regression.ipynb   # Logistic Regression model training and evaluation
│   ├── SVM.ipynb                   # Support Vector Machine training and evaluation
│   ├── Random forest.ipynb         # Random Forest training and evaluation
│   └── Deep learning.ipynb         # Deep learning pipeline and comparison
├── dataset/
│   └── home_value_prediction.csv   # Raw dataset
├── features/                       # Saved feature vectors (.npy / .h5)
├── reports/                        # Report
└── README.md
```

---

##How to Run the Notebooks

### Prerequisites

Make sure the following libraries are installed before running any notebook:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
# For the deep learning notebook:
pip install torch torchvision  # or: pip install tensorflow
```
### Step-by-step Instructions

1. **Clone this repository:**
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Ensure the dataset is in place:**  
   The file `dataset/home_value_prediction.csv` must exist before running any notebook. If not present, download it from [[home_dataset](https://drive.google.com/drive/folders/1U2cwVZdXZoC18OTrUl3rU9ZIzJStWOh-)].

3. **Run notebooks in the following order:**

   | Step | Notebook | Description |
   |------|----------|-------------|
   | 1 | `src/EDA+preprocessing.ipynb` | **Run this first.** Performs EDA and outputs cleaned/preprocessed data used by all model notebooks. |
   | 2 | `src/logistic regression.ipynb` | Trains and evaluates Logistic Regression with multiple configurations. |
   | 3 | `src/SVM.ipynb` | Trains and evaluates SVM with different kernels and parameters. |
   | 4 | `src/Random forest.ipynb` | Trains and evaluates Random Forest with varying hyperparameters. |
   | 5 *(optional)* | `src/Deep learning.ipynb` | Implements deep learning pipeline and compares with traditional ML. |

4. **In each notebook**, use **Runtime → Run all** (Google Colab) or **Kernel → Restart & Run All** (Jupyter) to execute all cells.

**Note:** Run `EDA+preprocessing.ipynb` before any model notebook, as it generates the preprocessed data and saved features used downstream.

---

## Dataset

- **Name:** Home Value Prediction  
- **File:** `dataset/home_value_prediction.csv`  
- **Description:** Tabular dataset for predicting home values, containing numerical and categorical features with missing values.

---

## Notes
- This project is part of the CO3117 Machine Learning course at HCMUT, VNU-HCM.
