# Tumor Detection Project

## Overview
This project classifies tumors as **Malignant (M)** or **Benign (B)** using machine learning.  
We apply a **Random Forest Classifier** to the Tumor Detection dataset and analyze important features that influence diagnosis.

## Dataset
- **File:** Tumor_Detection.csv  
- Contains features like `mean radius`, `mean texture`, `mean perimeter`, etc.  
- Target: `diagnosis` (M=Malignant, B=Benign).  

## Methodology
1. **Data Cleaning**
   - Dropped irrelevant columns (`id`, `Unnamed: 32`).  
   - Checked for missing values.  
2. **EDA**
   - Count plot for diagnosis distribution.  
   - Correlation heatmap between features.  
   - Distribution plots for key attributes.  
3. **Preprocessing**
   - Encoded labels (M=1, B=0).  
   - Standardized features using `StandardScaler`.  
   - Train-test split (80-20).  
4. **Model**
   - Applied **Random Forest Classifier** (`sklearn`).  
   - Evaluated using accuracy, classification report, and confusion matrix.  
5. **Feature Importance**
   - Identified top predictors of tumor malignancy.  

## Results
- Achieved **high accuracy (>90%)** on test data.  
- Top features: `mean radius`, `mean perimeter`, `mean concavity`.  

## How to Run
```bash
git clone https://github.com/your-username/Tumor_Detection-project.git
cd Tumor_Detection-project
pip install -r requirements.txt
jupyter notebook Tumor_Detection_Project.ipynb
