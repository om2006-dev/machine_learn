# 📈 Machine Learning: Predictive Modeling & Advanced Feature Engineering

This repository contains an end-to-end data science workflow focused on building high-performance predictive models. The project bridges the gap between raw, messy data and accurate machine learning predictions by implementing robust feature engineering techniques and linear regression architectures.

---

## 🛠️ Key Project Components

### 1. Advanced Feature Engineering & Preprocessing
Data quality is the foundation of any ML model. This project addresses common real-world data challenges:
*   **Handling Class Imbalance:** Implemented **SMOTE (Synthetic Minority Over-sampling Technique)** to synthesize new examples for minority classes, preventing model bias towards majority labels.
*   **Missing Data Imputation:** Developed automated strategies for detecting and filling missing values (Mean/Median/Mode) to maintain dataset integrity.
*   **Outlier Detection:** Used statistical methods to identify and handle anomalies that could skew model training.
*   **Scalability:** Designed modular scripts for data cleaning that can be integrated into production pipelines.

### 2. Predictive Analytics (Linear Regression)
Built and optimized multiple regression models to predict continuous numerical values (e.g., Economic Indices, Physical Metrics):
*   **Simple & Multiple Linear Regression:** Leveraged **OLS (Ordinary Least Squares)** to model relationships between dependent and independent variables.
*   **Polynomial Regression:** Addressed non-linear relationships by transforming features into higher-degree polynomials.
*   **Performance Evaluation:** Validated models using metrics like **R-squared**, **Adjusted R-squared**, and **MSE (Mean Squared Error)**.
*   **Visualization:** Created detailed correlation heatmaps and residual plots using **Seaborn** and **Matplotlib** to confirm model assumptions (homoscedasticity, linearity).

---

## 📂 Repository Structure

```text
├── feature engineering/
│   ├── imbalance_data_smote.ipynb  # Class imbalance handling with SMOTE
│   ├── missing_data.ipynb          # Imputation techniques
│   └── ...
├── linear_regression_practical/
│   ├── economic_index.csv          # Macroeconomic dataset
│   ├── height-weight.csv           # Physical metrics dataset
│   ├── ols.ipynb                   # OLS regression implementation
│   ├── multiple_lr.ipynb           # Multi-variable modeling
│   └── poly_reg.ipynb              # Non-linear regression
└── requirements.txt                # Environment dependencies
```

---

## 🚀 Getting Started

### Prerequisites
*   Python 3.8+
*   Jupyter Notebook / VS Code (with Jupyter extension)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Notebooks
Launch Jupyter and navigate to either `feature engineering/` or `linear_regression_practical/` to explore the implementations:
```bash
jupyter notebook
```

---

## 🧰 Tech Stack
*   **Languages:** Python
*   **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Imbalanced-learn (SMOTE)
*   **Environment:** Jupyter Notebooks

---

## 📊 Key Insights
*   **Data Quality Matters:** Applying SMOTE to imbalanced datasets significantly improved the recall for minority classes compared to baseline models.
*   **Feature Selection:** Through EDA, identified critical economic indicators that showed a >0.8 correlation with the target index, leading to a more efficient and interpretable multiple regression model.
