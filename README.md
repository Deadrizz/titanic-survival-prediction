# Titanic Survival Prediction

This project aims to build and evaluate machine learning models to predict the survival of passengers aboard the Titanic using the Titanic dataset.

## 📊 Dataset

The dataset is loaded using `seaborn`'s built-in Titanic dataset. It includes various features such as:
- Age
- Sex
- Passenger Class (Pclass)
- Number of siblings/spouses (SibSp)
- Number of parents/children (Parch)
- Embarked location
- Survival status (target variable)

## 🔧 Preprocessing

- Missing values in the `age` column were filled with the mean.
- One-hot encoding was applied to categorical columns (`sex`, `embarked`).
- Additional features were engineered:
  - `FamilySize`
  - `IsAlone`
  - `IsChild`
- Numerical features were scaled using `StandardScaler`.

## 📈 Models

Three classification models were trained and evaluated:
- Logistic Regression
- Random Forest Classifier
- Gradient Boosting Classifier

## ✅ Evaluation

- Accuracy, Precision, Recall, and F1 Score were calculated.
- Confusion Matrices were generated.
- Cross-validation was used to evaluate model robustness.
- `GridSearchCV` was used to fine-tune the Random Forest model.

## 🧪 Best Model

Random Forest showed the best performance after hyperparameter tuning.

## 📦 Requirements

See [requirements.txt](./requirements.txt) for a list of dependencies.

## 🧠 Author

Built by a junior data enthusiast for educational purposes and portfolio development.
