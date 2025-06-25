## 🎯 Objectives

The primary objectives of this project are:

- To load and explore the **Titanic dataset** (`titanic.csv`) using Pandas.
- To handle missing data:
  - Impute missing `Age` values using the median.
  - Impute missing `Embarked` values using the mode.
  - Drop the `Cabin` column due to excessive missing values.
- To perform data cleaning and type conversions:
  - Convert `Fare` to float and `Pclass` to integer for consistency.
- To conduct **feature engineering**:
  - Extract titles (e.g., Mr., Miss, etc.) from the `Name` field into a new column `Title`.
  - Create an `Age_Group` feature by binning age into categories: Child, Teen, Young Adult, Middle Aged, and Senior.
- To encode categorical variables using one-hot encoding:
  - Apply `pd.get_dummies()` to features like `Sex`, `Embarked`, and `Title`, dropping the first category to avoid multicollinearity.
- To prepare a final cleaned dataset for future machine learning modeling by:
  - Dropping irrelevant or redundant columns: `Name`, `Ticket`, and `PassengerId`.
  - Ensuring no missing values remain.

This structured approach ensures the dataset is clean, consistent, and enriched with meaningful features for modeling survival predictions.
