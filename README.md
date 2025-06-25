# DATA-PREPROCESSING-AND-FEATURE-ENGINEERING-ON-TITANIC-DATASET
# 🚢 Titanic Dataset - Data Preprocessing & Feature Engineering

This project involves cleaning, transforming, and preparing the Titanic dataset (`titanic.csv`) for future machine learning tasks. It demonstrates effective **data preprocessing**, **missing value treatment**, and **feature engineering** using Python and Pandas.

---

## 📁 Files Included

- `titanic.csv` – Dataset used for preprocessing
- `titanic_preprocessing.ipynb` – Jupyter Notebook or Python script (your code)
- `README.md` – Project overview and instructions

---

## 🎯 Objectives

The primary objectives of this project are:

- To load and explore the **Titanic dataset** using Pandas.
- To handle missing data:
  - Impute missing `Age` values using the median.
  - Impute missing `Embarked` values using the mode.
  - Drop the `Cabin` column due to excessive missing values.
- To conduct data cleaning and type conversions:
  - Convert `Fare` to float and `Pclass` to integer.
- To perform **feature engineering**:
  - Extract `Title` from the `Name` field.
  - Create `Age_Group` by binning age into categories: Child, Teen, Young Adult, Middle Aged, and Senior.
- To encode categorical variables using one-hot encoding:
  - `Sex`, `Embarked`, and `Title`, with `drop_first=True`.
- To drop unnecessary or redundant columns:
  - `Name`, `Ticket`, and `PassengerId`.

---

## 🔍 Exploratory Data Analysis (EDA)

Initial steps before preprocessing:

- Inspected the dataset structure using `.head()` and `.info()`.
- Checked for missing values using `.isnull().sum()`.
- Observed variable distributions (like `Age`, `Fare`, and `Pclass`).
- Verified categorical variables such as `Sex`, `Embarked`, and extracted `Title`.

---

## 🧹 Preprocessing Summary

| Task                       | Technique Used                 |
|---------------------------|-------------------------------|
| Handle missing `Age`      | Fill with median              |
| Handle missing `Embarked` | Fill with mode                |
| Drop `Cabin`              | Excessive missing values      |
| Convert `Fare`            | Cast to `float`               |
| Convert `Pclass`          | Cast to `int`                 |
| Extract `Title`           | Regex from `Name` column      |
| Create `Age_Group`        | `pd.cut()` with labeled bins  |
| Encode categoricals       | `pd.get_dummies()`            |
| Drop extra columns        | `Name`, `Ticket`, `PassengerId`|

---

## 📦 Libraries Used

- `pandas`
- `numpy`
- `seaborn` *(optional for EDA/visualization)*
- `matplotlib` *(optional)*

---

## ▶️ How to Run

1. Open the notebook in Google Colab or Jupyter Notebook.
2. Upload the `titanic.csv` file when prompted.
3. Run the cells step by step to see the cleaning and transformation process.
4. The final cleaned dataset is displayed using `.head()`.

---

## ✅ Final Output

- A clean, well-structured dataset with no missing values.
- Feature-rich dataset ready for building classification models (e.g., logistic regression, decision trees, etc.).

---

## 📝 Next Steps (Suggestions)

- Perform data visualization (e.g., survival rate by title, age group, sex).
- Build and evaluate predictive models (e.g., logistic regression, random forest).
- Use cross-validation to test model accuracy.

---

## 🤝 Contributing

Feel free to fork this repository and suggest improvements or add modeling layers.

---

## 📃 License

This project is open-source and available under the [MIT License](LICENSE).
