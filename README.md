# Titanic-Dataset
 Predict passenger survival on the Titanic using a dataset containing features such as passenger class, age, fare, and more. Approach:  Performed data preprocessing (handling missing values, encoding categorical features).  Explored data using visualizations. Trained and evaluated machine learning models (Random Forest and Logistic Regression).
# Titanic Survival Classification Project

![Titanic](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fd/RMS_Titanic_3.jpg/1200px-RMS_Titanic_3.jpg)

## Project Overview
This project implements machine learning models to predict passenger survival on the Titanic based on features like passenger class, age, gender, and fare. The goal is to demonstrate data preprocessing, feature engineering, model training, and evaluation techniques.

## Dataset
The dataset used is from Kaggle:  
[Titanic Dataset](https://www.kaggle.com/datasets/yasserh/titanic-dataset)

Features include:
- Passenger class (Pclass)
- Name
- Sex
- Age
- Fare
- Embarked port
- And more...

## Project Structure
titanic-dataset/
├── data/ # Raw and processed data
│ ├── train.csv # Training data
│ └── test.csv # Testing data
├── notebooks/ # Jupyter notebooks
│ └── titanic_analysis.ipynb
├── src/ # Source code
│ ├── preprocessing.py # Data cleaning
│ ├── models.py # ML models
│ └── evaluation.py # Model evaluation
├── reports/ # Generated reports
├── README.md # This file
└── requirements.txt # Dependencies

## Key Steps
1. **Data Preprocessing**:
   - Handled missing values (Age, Embarked)
   - Encoded categorical features (Sex, Embarked)
   - Dropped irrelevant columns (PassengerId, Name, etc.)

2. **Feature Engineering**:
   - Created new features (FamilySize, Title extraction)
   - Normalized numerical features

3. **Models Implemented**:
   - Random Forest Classifier
   - Logistic Regression
   - Hyperparameter tuning with GridSearchCV

4. **Evaluation Metrics**:
   - Accuracy: 79.33% (Random Forest)
   - Precision, Recall, F1-score
   - Confusion matrices

## Results
| Model               | Training Accuracy | Test Accuracy |
|---------------------|-------------------|---------------|
| Random Forest       | 97.75%            | 79.33%        |
| Logistic Regression | 79.49%            | 79.89%        |

## How to Run
1. Clone repository:
   ```bash
   git clone https://github.com/abubakar150/Titanic-Dataset.git
   cd Titanic-Dataset
