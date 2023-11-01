# Titanic Dataset Analysis

This repository contains code for the analysis of the Titanic dataset. The dataset is loaded using the Pandas library in Python and then subjected to both non-graphical (numerical) and graphical (visual) analysis. The analysis aims to explore the dataset, identify missing values, and perform multivariate analysis, including correlations and scatterplots.

## Dataset Information

The dataset used for this analysis is stored in a CSV file named "Titanic.csv." It contains information about passengers on the Titanic, including details such as age, class, fare, and whether they survived or not. The dataset is loaded into a Pandas DataFrame for analysis.

### Data Summary

To get a quick overview of the dataset, the following operations are performed:
- `df.info()`: This command displays basic information about the DataFrame, including the number of entries, data types, and memory usage.
- `df.isnull().sum()`: This command checks for missing values in the dataset, providing insights into the columns with missing data.

### Multivariate Analysis

Multivariate analysis aims to explore the relationships between multiple variables in the dataset.

#### Multiple Numerical Variables

The following analyses are performed on multiple numerical variables:
- `df.corr()`: This command calculates the correlation matrix between numerical variables, showing how they are related to each other.
- `sns.heatmap()`: This command generates a heatmap of the correlation matrix, providing a visual representation of the relationships.
- `df['Pclass'].value_counts()`: This command counts the occurrences of passenger class (Pclass) to understand the distribution.

#### Correlation with Age

The correlation between the "Age" variable and other numerical variables is explored using `df.corrwith(df['Age'])`. This provides insights into how age is related to other features.

#### Scatterplots

Scatterplots are used to visualize relationships between numerical and categorical variables as well as numerical variables.

- `sns.regplot()`: This command creates scatterplots to visualize relationships between age and fare, as well as passenger class and fare.
- `sns.scatterplot()`: This command creates scatterplots to visualize the relationship between age and fare while using the "Embarked" variable for color differentiation.

## Conclusions

1. The dataset contains information about passengers on the Titanic, including details on age, class, fare, and survival status.

2. There are missing values in some columns, which may need to be handled in subsequent data preprocessing steps.

3. The correlation analysis shows that passenger class (Pclass) is negatively correlated with fare, indicating that higher-class passengers paid more for their tickets. Age has relatively weak correlations with other numerical variables.

4. Scatterplots reveal insights into relationships between variables. For instance, the scatterplot of age and fare shows a positive trend, indicating that as age increases, fare tends to increase. Additionally, passenger class and fare are visualized, showing that higher-class passengers generally paid more for their tickets.

5. The scatterplot using "Embarked" as a hue suggests that the embarkation location might influence the age and fare relationship. Further analysis could explore this relationship in more detail.

This analysis provides a foundational understanding of the Titanic dataset, uncovering potential relationships and insights that can be further explored and used for predictive modeling or other data-driven tasks.

