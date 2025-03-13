# DAI-101 Assignment 23321022
 
Life Expectancy Dependence Factors, Data Analysis and Predictions


This analysis investigates the factors influencing life expectancy across different countries in 2015. The dataset includes socio-economic, health, and demographic variables such as GDP, healthcare expenditure, schooling, and mortality rates, etc. The goal is to clean the data, analyze patterns, and explore relationships between variables to understand their impact on life expectancy.

DATASET: https://www.kaggle.com/code/michau96/what-does-life-expectancy-depend-on-4d-charts/notebook
DEPENDENCIES: pip install pandas numpy matplotlib seaborn

1. Data Cleaning
   

1.1 Handling Missing Values


Missing values were detected in several columns, particularly Alcohol Consumption, GDP, and Healthcare Expenditure.

Numerical missing values were imputed using the median to avoid skewing the data.

1.2 Removing Duplicates


Duplicate rows were identified and removed to prevent redundancy.

1.3 Outlier Detection and Treatment


The Interquartile Range (IQR) method was used to detect and cap outliers for numerical variables such as GDP, Life Expectancy, and Schooling.

Box plots were used before and after capping to visualize changes.

2. Exploratory Data Analysis (EDA)



2.1 Univariate Analysis


Summary Statistics: The mean, median, standard deviation, skewness, and kurtosis were computed for all numerical variables.

Histograms: Used to analyze the distribution of key variables like Life Expectancy, GDP, and Schooling.

Categorical Frequency Distribution: The dataset contains two primary categories for the Status column: Developed and Developing countries, with more entries for developing nations.

2.2 Bivariate Analysis


Correlation Matrix & Heatmap:

Strong positive correlation between Schooling and Life Expectancy (r ≈ 0.78).

Strong negative correlation between Adult Mortality and Life Expectancy (r ≈ -0.85).

GDP and Healthcare Expenditure showed moderate positive correlations with Life Expectancy.

Scatter Plots:

Confirmed linear relationships between Life Expectancy and variables like Income Composition of Resources.

Bar Plots & Violin Plots:

Showed differences in life expectancy distribution between developed and developing countries.

2.3 Multivariate Analysis


Pair Plots: Examined relationships between multiple numerical variables, highlighting clusters of developed vs. developing countries.

Grouped Comparisons:

The top 10 countries with the highest life expectancy were visualized.

A heatmap showed how income composition and healthcare expenditure and other factors influence life expectancy.

3. Conclusion



Life Expectancy is highly influenced by healthcare expenditure, education levels, and economic factors.

Developing countries generally have lower life expectancy due to higher adult mortality and lower access to healthcare.

Policies focusing on education, healthcare funding, and economic development could significantly improve life expectancy globally.
