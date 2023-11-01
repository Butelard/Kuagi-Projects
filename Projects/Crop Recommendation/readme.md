# Crop Recommendation Data Analysis

This repository contains code for analyzing a dataset related to crop recommendation. The dataset is loaded using the Pandas library in Python and then subjected to both non-graphical (numerical) and graphical (visual) analysis. The primary goal of this analysis is to gain insights into the data, its structure, and the distribution of its various features.

## Dataset Information

The dataset used for this analysis is stored in a CSV file named "Crop_recommendation.csv." It contains information related to crops and their recommendations. The dataset is loaded into a Pandas DataFrame for analysis.

### Quick Data Summary

To get a quick overview of the dataset, the following operations are performed:
- `df.info()`: This command displays basic information about the DataFrame, including the number of entries, data types, and memory usage.
- `df.isnull().sum()`: This command checks for missing values in the dataset. In this case, there are no missing values in the dataset.

### Univariate Analysis

Univariate analysis is conducted to understand the characteristics of individual variables within the dataset. The analysis includes both non-graphical and graphical aspects.

#### Non-Graphical Analysis

The following non-graphical analysis is performed:
- `df.describe()`: This command provides statistical summaries for the numerical columns in the dataset, such as count, mean, standard deviation, minimum, and maximum values.
- `df["label"].nunique()`: This command calculates the number of unique crop labels in the dataset. There are 22 different crops in the data.
- `df["label"].unique()`: This command displays the unique crop labels in the dataset.
- `df["label"].value_counts()`: This command counts the occurrences of each crop label in the dataset.

#### Univariate Graphical Analysis

Graphical analysis is used to visualize the data and gain insights into the distribution of numerical and categorical features.

##### Numerical Features

The following visualizations are created for numerical features:
- Kernel Density Estimation (KDE) plots using `sns.kdeplot()`: These plots show the distribution of numerical features.
- Histograms using `sns.histplot()`: These plots provide a histogram representation of numerical features.
- Box plots using `sns.boxplot()`: These plots help identify outliers and visualize the distribution of numerical features.

##### Categorical Features

For the categorical feature "label," a count plot is created using `sns.countplot()`. This plot displays the frequency of each crop in the dataset.

## Installation

To run this analysis, you need Python and the following libraries installed:
- Pandas
- Matplotlib
- Seaborn

##Author
This code was written by [Dayyabu Abdulrazak].
