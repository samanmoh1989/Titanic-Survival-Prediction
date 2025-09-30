# Titanic Survival Prediction 🚢
![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![scikit--learn](https://img.shields.io/badge/scikit--learn-1.4+-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Kaggle Dataset](https://img.shields.io/badge/Data-Kaggle-blue.svg)
This project applies **Data Science and Machine Learning** techniques to predict the survival of Titanic passengers using the famous [Kaggle Titanic dataset](https://www.kaggle.com/c/titanic).

---

## 📊 Project Workflow
1. **Data Cleaning**
   - Filled missing `Age` with median  
   - Filled missing `Embarked` with mode  
   - Dropped `Cabin` due to too many missing values  

2. **Exploratory Data Analysis (EDA)**
   - Survival rates by `Sex`, `Pclass`, `Age`, and `FamilySize`  
   - Visualizations with Seaborn & Matplotlib  

3. **Feature Engineering**
   - `FamilySize` and `IsAlone`  
   - Extracted `Title` from passenger names (Mr, Miss, Mrs, etc.)  
   - `FareBand` (Low, Medium, High, Very High)  
   - One-hot encoding of categorical features  

4. **Modeling**
   - Logistic Regression → Accuracy ≈ 0.80  
   - Random Forest → Accuracy ≈ 0.83  
   - XGBoost → Accuracy ≈ 0.82  

5. **Results**
   - Best model: **Random Forest** (~83% accuracy)  
   - Most important features: `Sex`, `Pclass`, `Fare`, `Title`, `FamilySize`  

---

## 📈 Visualizations
Examples of outputs generated in the notebook:

- Confusion Matrices for all models  
- Feature importance (Random Forest & XGBoost)  

*(You can add PNG images here with `![caption](path/to/img.png)` if you export plots)*  

---

## 🚀 How to Run
```bash
# clone the repository
git clone https://github.com/samanmoh1989/Titanic-Survival-Prediction.git
cd Titanic-Survival-Prediction

# install dependencies
pip install -r requirements.txt

# run the notebook
jupyter notebook Titanic.ipynb
