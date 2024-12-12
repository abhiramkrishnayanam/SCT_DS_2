# SCT_DS_2
## Exploratory data analysis in Titanic dataset
# Titanic Data Analysis: Data Cleaning and Exploratory Data Analysis (EDA)

## Overview
The Titanic dataset is a widely used dataset for learning data analysis and machine learning. It contains information about the passengers aboard the Titanic, including demographic details, ticket class, and survival status. This project focuses on performing data cleaning and exploratory data analysis (EDA) to uncover trends and patterns in the dataset.

---

## Objectives
1. **Data Cleaning**: 
   - Handle missing values.
   - Ensure consistency in data formats.
   - Prepare the dataset for further analysis.
2. **Exploratory Data Analysis (EDA)**:
   - Visualize trends and relationships.
   - Identify patterns that affect survival rates.
   - Gain insights for predictive modeling.

---

## Steps Undertaken

### 1. Data Cleaning

#### **Missing Values**:
- **Age**: Imputed missing values using the median or group-specific medians (e.g., based on passenger class and gender).
- **Embarked**: Filled missing values with the mode (most frequent value).
- **Cabin**: Dropped due to a high percentage of missing values or categorized as "Unknown" for further analysis.

#### **Data Consistency**:
- Ensured uniform formatting for categorical variables like `Sex` and `Embarked`.
- Standardized column names for readability.

#### **Outlier Detection**:
- Identified outliers in numerical columns such as `Fare` and `Age` using visualization techniques (e.g., box plots).
- Applied transformations or removed extreme outliers if necessary.

#### **Encoding**:
- Converted categorical variables (e.g., `Sex`, `Embarked`) into numerical representations for correlation analysis and visualization.

---

### 2. Exploratory Data Analysis (EDA)

#### **Univariate Analysis**:
- Examined the distribution of individual variables such as `Age`, `Fare`, `Pclass`, and `Survived` using histograms and bar charts.
- Identified key characteristics, such as:
  - The majority of passengers were in the 3rd class.
  - More passengers embarked from Southampton (S).

#### **Bivariate Analysis**:
- Explored relationships between two variables using visualizations:
  - **Survival vs. Gender**: Women had a significantly higher survival rate compared to men.
  - **Survival vs. Pclass**: Passengers in 1st class had a higher survival rate than those in 2nd or 3rd class.
  - **Survival vs. Fare**: Higher fares were associated with better survival rates.

#### **Multivariate Analysis**:
- Investigated the interaction of multiple variables:
  - Combined `Pclass`, `Sex`, and `Age` to understand survival probabilities for different groups.
  - Analyzed the combined effect of `Embarked`, `Fare`, and `Pclass` on survival.

#### **Correlation Analysis**:
- Created a correlation matrix for numerical features to identify significant relationships.
  - Found correlations between `Fare` and `Survived`.
  - Highlighted weak or no correlation with features like `Ticket`.

---

## Key Insights
- **Gender**: Women were more likely to survive than men.
- **Class**: Higher-class passengers (1st and 2nd) had better survival rates.
- **Age**: Children (younger passengers) had higher survival rates.
- **Fare**: Passengers with higher fares were more likely to survive.
- **Embarkation**: Passengers who embarked from Cherbourg (C) had slightly higher survival rates.

---

## Tools Used
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn.
- **Environment**: Jupyter Notebook or any Python IDE.
- **Visualization Techniques**: Histograms, bar charts, box plots, heatmaps.

---

## Future Work
- Build predictive models using the cleaned dataset.
- Explore advanced feature engineering techniques.
- Compare survival trends across different machine learning algorithms.

---

## Dataset Source
The Titanic dataset is available on [Kaggle](https://www.kaggle.com/c/titanic/data) and contains the following columns:
- `PassengerId`: Unique ID for each passenger.
- `Survived`: Survival status (0 = No, 1 = Yes).
- `Pclass`: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd).
- `Name`: Name of the passenger.
- `Sex`: Gender.
- `Age`: Age of the passenger.
- `SibSp`: Number of siblings/spouses aboard.
- `Parch`: Number of parents/children aboard.
- `Ticket`: Ticket number.
- `Fare`: Ticket fare.
- `Cabin`: Cabin number.
- `Embarked`: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton).

---

## Conclusion
This project provided a comprehensive understanding of the Titanic dataset, focusing on cleaning and analyzing the data to uncover patterns and trends related to survival. These insights can guide further predictive modeling efforts and serve as a foundation for similar analyses.
