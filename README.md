# Breast Cancer Prediction Project  

## Author  
Kenneth Ronald Kiplagat  

---

##  Project Overview  
This project applies the **CRISP-DM methodology** to the Breast Cancer dataset (available in `sklearn.datasets`).  
The main goal is to **predict whether a tumor is malignant or benign** using machine learning techniques.  

The process covers the complete data science pipeline:  
1. **Business Understanding**  
2. **Data Understanding**  
3. **Data Preparation (Cleaning & Transformation)**  
4. **Exploratory Data Analysis (EDA)**  
5. **Modeling**  
6. **Evaluation**  

---

##  Dataset  
- Source: `sklearn.datasets.load_breast_cancer`  
- Size: **569 samples, 30 features**  
- Target Variable:  
  - `0` = Malignant  
  - `1` = Benign  

---

##  Methodology (CRISP-DM Steps)  

### 1. Business Understanding  
- Breast cancer diagnosis is a critical medical task.  
- Early and accurate prediction can support doctors in decision-making.  
- Objective: Build a classification model to predict malignancy.  

### 2. Data Understanding  
- Examined the dataset’s shape, column types, and target distribution.  
- Observed **balanced classes** (212 malignant, 357 benign).  

### 3. Data Preparation  
- Checked for missing values (none found).  
- Standardized the features for better model performance.  
- Split dataset into **train (80%) and test (20%)**.  

### 4. Exploratory Data Analysis (EDA)  
- Correlation analysis to detect multicollinearity.  
- Histograms, pair plots, and heatmaps to visualize distributions.  
- Observed strong correlation between mean radius, perimeter, and area.  

### 5. Modeling  
- Implemented a **Logistic Regression model**.  
- Chosen for its interpretability and baseline performance.  

### 6. Evaluation  
- Metrics: **Accuracy, Precision, Recall, F1-score, Confusion Matrix**.  
- Logistic Regression achieved:  
  - Accuracy ≈ **95%**  
  - High recall (important in medical diagnosis).  

---

## ⚙️ Tools & Libraries  
- **Python**  
- **Jupyter Notebook**  
- Libraries:  
  - `pandas`  
  - `numpy`  
  - `matplotlib`  
  - `seaborn`  
  - `scikit-learn`  

---

##  Results & Insights  
- The model demonstrates strong predictive power.  
- Feature scaling improved performance.  
- Important features include:  
  - Mean radius  
  - Mean texture  
  - Mean perimeter  
- The project proves that simple models can yield reliable results when the dataset is well-structured.  

---

##  Next Steps  
- Try advanced models: Random Forest, Gradient Boosting, SVM.  
- Use cross-validation for robustness.  
- Deploy the model using Flask or Streamlit for real-world application.  

