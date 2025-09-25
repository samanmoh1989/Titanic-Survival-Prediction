# Titanic Survival Prediction 🚢

This project applies **Data Science and Machine Learning** techniques to predict survival of passengers on the Titanic using the famous Kaggle dataset.

## 📊 Project Workflow
1. **Data Cleaning**
   - Filled missing `Age` with median
   - Filled missing `Embarked` with mode
   - Dropped `Cabin` due to too many missing values

2. **Exploratory Data Analysis (EDA)**
   - Survival rates by sex, passenger class, age, and family size
   - Visualization with Seaborn & Matplotlib

3. **Feature Engineering**
   - Created `FamilySize` and `IsAlone`
   - Extracted passenger `Title` from names (Mr, Miss, Mrs, etc.)
   - Created `FareBand` (Low, Medium, High, Very High)
   - One-hot encoded categorical features

4. **Modeling**
   - Logistic Regression (Accuracy ≈ 0.80)
   - Random Forest (Accuracy ≈ 0.83)
   - XGBoost (Accuracy ≈ 0.82)

5. **Results**
   - Best performance: **Random Forest** (≈ 83% accuracy)
   - Most important features: `Sex`, `Pclass`, `Fare`, `Title`, and `FamilySize`

## 📈 Visualizations
- Confusion matrices for all models
- Feature importance (Random Forest & XGBoost)

## 🚀 How to Run
```bash
git clone https://github.com/your-username/Titanic-Survival-Prediction.git
cd Titanic-Survival-Prediction
pip install -r requirements.txt
jupyter notebook Titanic.ipynb
