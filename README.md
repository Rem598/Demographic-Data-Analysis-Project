# Demographic-Data-Analysis-Project

A comprehensive statistical analysis project exploring descriptive statistics, distribution characteristics, and relationships between key demographic variables in a dataset of 5,000 respondents.

## Project Overview

This project focuses on analyzing a demographic dataset to understand the distribution of key variables, check for outliers, and determine if significant relationships exist between various categorical and numerical features. The analysis utilizes descriptive statistics, visualization techniques (histograms and boxplots), and inferential statistics (Chi-Square tests).

## Data Source

The analysis is based on the `Demographic_data.csv` file.

| Column Name | Data Type | Description |
| :--- | :--- | :--- |
| `Respondent_ID` | int64 | Unique identifier for each respondent. |
| `Age` | int64 | The age of the respondent. |
| `Gender` | object | Categorical: Female, Male, Other. |
| `Education_Level` | object | Categorical: Bachelor's, High School, Master's, PhD. |
| `Employment_Status` | object | Categorical: Employed, Retired, Student, Unemployed. |
| `Marital_Status` | object | Categorical: Divorced, Married, Single, Widowed. |
| `Household_Income` | int64 | The annual income of the respondent's household. |
| `Region` | object | Categorical: Central, East, North, South, West. |
| `Owns_Home` | object | Categorical: Yes/No. |
| `Has_Children` | object | Categorical: Yes/No. |
| `Internet_Usage_Hours` | int64 | Weekly internet usage in hours. |
| `Political_Affiliation` | object | Categorical: Conservative, Independent, Liberal, Other. |

## Analysis Objectives

1.  **Exploration (Descriptive Statistics):** Calculate measures of central tendency, dispersion, and shape for numerical variables like Age, Household Income, and Internet Usage Hours.
2.  **Distribution Assessment:** Visualize and describe the distribution of Age and Internet Usage Hours using Histograms.
3. **Outlier Check:** Use descriptive statistics and boxplots to identify extreme values in Household Income.
4.  **Relationship Analysis (Crosstabs & Chi-Square):** Test for relationships between pairs of categorical variables, including:
    * Gender and Marital Status.
    * Region and Home Ownership.
    * Employment Status and Education Level.
    * Age (Binned) and Has Children.
    * Political Affiliation and Region.

## Key Findings

### Descriptive Analysis Summary

* **Age:** The distribution of age appears to be normal and symmetrical. The key statistics are:
    * Mean: $43.58$ 
    * Median: $43.00$ 
    * Standard Deviation: $14.919$
* **Household Income:** The income range is from a minimum of $\$20,016$ to a maximum of $\$149,997$.No outliers were found in Household Income.
* **Internet Usage Hours:** The distribution is fairly uniform and very close to being symmetrical.
    * Skewness: $0.014$ 
    * Kurtosis: $-1.191$ 

### Relationship Analysis Summary

The analysis found that many key demographic variables are independent of each other.

| Relationship | Chi-Square ($\chi^2$) Value | Degrees of Freedom (df) | $p$-value | Conclusion (Significance at $\alpha=0.05$) | Source |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Region \* Owns Home** | $3.233$ | $4$ | $.520$ | **Not Significant**  |
| **Employment Status \* Education Level** | $15.289$ | $9$ | $.083$ | **Not Significant** |
| **Political Affiliation \* Region** | $15.845$ | $12$ | $.198$ | **Not Significant**|
| **Age (Binned) \* Has Children** | $.411$ | $3$ | $.938$ |**Not Significant** |

The only notable finding regarding the binned age group and children is that the **45-60 age group** has the highest percentage (50.2%) of respondents with children.

## Real-World Applications

The findings provide valuable insights for strategic planning:

* **Marketing Targeting:** A company selling family-oriented products could focus its marketing efforts on the **45-59 age group**, as this group has the highest percentage of respondents with children.
* **Policy Making:** The lack of a significant relationship between region and homeownership suggests that housing policy initiatives aimed at increasing homeownership should be broad and not solely focused on specific geographical regions.

---
