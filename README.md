# 🕵️‍♂️Los Angeles-Crime-Detection


## 🎯 Project Overview
This project focuses on predicting crime categories based on various features related to crime incidents. The goal is to develop a machine learning model that can accurately classify crime types, which could be valuable for law enforcement and urban planning.

## 📊 Dataset
The dataset includes information about crime incidents, such as:
- 📍 Location details (Latitude, Longitude, Area)
- 🕒 Temporal information (Date Reported, Date Occurred)
- 👤 Victim information (Age, Sex, Descent)
- 🔍 Crime details (Modus Operandi, Premise, Weapon Used)

## 🧹 Data Preprocessing
1. **Handling Missing Values**:
   - 🗺️ Imputed missing latitude and longitude with mean values
   - ✅ Created binary features for cross-street presence and victim presence
   - 🔄 Filled missing categorical values with most frequent occurrences

2. **Feature Engineering**:
   - ⏳ Created 'Days_Lapsed' feature to capture time between occurrence and reporting
   - 🏷️ Transformed 'Modus_Operandi' using Multi-Label Binarization

3. **Categorical Encoding**:
   - 🔢 Used One-Hot Encoding for categorical features

## 🤖 Model Development
Three models were evaluated:
1. 🌳 Decision Tree Classifier
2. 📈 Logistic Regression
3. 🌲 Random Forest Classifier

The Random Forest Classifier performed best with the following parameters:
- n_estimators: 300
- min_samples_split: 2
- min_samples_leaf: 1
- max_depth: None
- bootstrap: False

## 📊 Results
- 🎉 Random Forest Classifier achieved 94.08% accuracy on the validation set

## 🚀 Future Improvements
- 🛠️ Explore more advanced feature engineering techniques
- 🧪 Investigate other algorithms like Gradient Boosting or Neural Networks
- 🔬 Perform more in-depth error analysis to understand misclassifications

## 🛠️ Tools and Libraries Used
- 🐍 Python
- 🐼 Pandas, 🔢 NumPy
- 🧠 Scikit-learn
- 📊 Matplotlib, Seaborn
