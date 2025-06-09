# 🚢 Titanic Survival Prediction

A machine learning project to predict whether a passenger survived the Titanic disaster using classification algorithms.

---

## 🧠 Overview

This project builds a predictive model that determines which passengers survived the Titanic shipwreck of 1912, based on features like age, sex, passenger class, fare, and embarkation point.

---

## 📂 Project Structure

1. **Data Import**  
   - The dataset includes `train.csv`, `test.csv`, and `gender_submission.csv` from the Kaggle Titanic competition.

2. **Exploratory Data Analysis (EDA)**  
   - Handle missing values (`Age`, `Embarked`, `Fare`).  
   - Analyze feature distributions and correlations with survival.

3. **Feature Engineering**  
   - Create new features:
     - **Title** extracted from names (`Mr.`, `Mrs.`, etc.)
     - **FamilySize** from `SibSp + Parch + 1`
   - Encode categorical variables (`Sex`, `Embarked`, `Title`) using Label Encoding or One-Hot Encoding.

4. **Model Building**  
   - Models used include:
     - Logistic Regression  
     - Random Forest Classifier  
     - K-Nearest Neighbors  
   - Hyperparameter tuning using `GridSearchCV`.

5. **Evaluation**  
   - Evaluate models using Accuracy, Precision, Recall, F1-score.  
   - Plot Confusion Matrix.

6. **Prediction and Submission**  
   - Generate `submission.csv` for Kaggle submission.

---

## ⚙️ Tools and Libraries

- Programming Language: Python  
- Libraries:
  - `pandas`, `numpy` for data processing  
  - `matplotlib`, `seaborn` for data visualization  
  - `scikit-learn` for model training and evaluation

---

## 📈 Results

- Best model: `Random Forest Classifier`  
- Accuracy achieved: approximately **82–84%** on validation data  
- Most important features: `Sex`, `Pclass`, `Age`, `FamilySize`, and `Title`

---

## ▶️ How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/HendRamadan1/Titanic-project.git
   cd Titanic-project
