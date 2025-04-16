# Analyzing and Modeling US Trade Deficits and Tariff Impacts: A Gradient Boosting Approach

This project provides a comprehensive analysis of international trade data focusing on the United States' 2024 trade deficits, import-export dynamics, and the impact of tariffs implemented under the Trump administration. The analysis employs advanced data science techniques, specifically Gradient Boosting, to model and interpret these economic relationships.

---

## 📂 Dataset Overview

The dataset comprises trade-related metrics between the US and various countries, including the trade deficit, export and import values, tariff rates alleged and responded to during Trump's administration, and population statistics for each country.

### **Dataset Sample**

| Country               | US 2024 Deficit | US 2024 Exports | US 2024 Imports (Customs Basis) | Trump Tariffs Alleged | Trump Response | Population |
|-----------------------|-----------------|-----------------|----------------------------------|-----------------------|----------------|------------|
| Afghanistan           | -11.1           | 11.4            | 22.6                             | 49%                   | 25%            | 41,454,761 |
| Albania               | 13.4            | 141.7           | 128.3                            | 10%                   | 10%            | 2,745,972  |
| Algeria               | -1,447.10       | 1,014.50        | 2,461.60                         | 59%                   | 29%            | 46,164,219 |
| Andorra               | 1.5             | 4.9             | 3.4                              | 10%                   | 10%            | 80,856     |
| Angola                | -1,186.90       | 682.4           | 1,869.20                         | 63%                   | 32%            | 36,749,906 |
| Anguilla              | 71.3            | 72.5            | 1.2                              | 10%                   | 10%            |             |
| Antigua and Barbuda   | 550             | 573.8           | 23.8                             | 10%                   | 10%            | 93,316     |
| Argentina             | 2,078.80        | 9,171.00        | 7,092.20                         | 10%                   | 10%            | 45,538,401 |

---

## 🚀 Project Workflow

The project followed a structured data analysis pipeline:

### **Data Preparation and Validation**
- Import and validate data integrity
- Inspect data types, missing values, formatting issues, duplicates, and outliers
- Perform exploratory statistics and visualization

### **Data Cleaning**
- Address missing data, correct formatting issues, and handle outliers
- Validate data cleaning procedures

### **Exploratory Data Analysis (EDA)**
- Correlation analysis
- Distribution analysis
- Multicollinearity assessment

### **Feature Engineering**
- Creation of meaningful features based on domain insights
- Feature selection to handle redundancy and multicollinearity

### **Modeling and Evaluation**
- Implementation of various regression models:
  - Linear Regression
  - Ridge Regression
  - Lasso Regression
  - Random Forest Regression
  - Gradient Boosting Regression
- Evaluation and comparison using Cross-Validation (R² metric)
- Selection of Gradient Boosting as the optimal model based on performance

### **Model Optimization**
- Hyperparameter tuning using GridSearchCV for the Gradient Boosting model
- Evaluation of optimized model performance on test data

### **Visualization and Interpretation**
- Detailed feature importance analysis
- Interpretation of model insights to highlight key determinants of US trade deficits

### **Deployment Preparation**
- Saving the final optimized model and preprocessing scaler for deployment purposes

---

## 🛠️ Tools and Technologies

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (GradientBoostingRegressor, GridSearchCV)
- Jupyter Notebook

---

## 📌 Usage Instructions

1. Clone this repository and navigate into the project directory:
   ```bash
   git clone https://github.com/deejayhighbee/Trade-Deficits-Tariff-Impacts-GB-Approach.git
   cd Trade-Deficits-Tariff-Impacts-GB-Approach
   pip install -r requirements.txt
   jupyter notebook
