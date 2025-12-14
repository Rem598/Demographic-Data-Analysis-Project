# Demographic-Data-Analysis-Project

A comprehensive statistical analysis project exploring descriptive statistics, distribution characteristics, and relationships between key demographic variables in a dataset of 5,000 respondents.

## Project Overview

This project focuses on analyzing a demographic dataset to understand the distribution of key variables, check for outliers, and determine if significant relationships exist between various categorical and numerical features. The analysis utilizes descriptive statistics, visualization techniques (histograms and boxplots), and inferential statistics (Chi-Square tests).

## Data Source

The analysis is based on the `week12_data.csv` file.

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

1.  [cite_start]**Exploration (Descriptive Statistics):** Calculate measures of central tendency, dispersion, and shape for numerical variables like Age, Household Income, and Internet Usage Hours[cite: 132].
2.  [cite_start]**Distribution Assessment:** Visualize and describe the distribution of Age and Internet Usage Hours using Histograms[cite: 155, 181].
3.  [cite_start]**Outlier Check:** Use descriptive statistics and boxplots to identify extreme values in Household Income[cite: 194, 207].
4.  **Relationship Analysis (Crosstabs & Chi-Square):** Test for relationships between pairs of categorical variables, including:
    * [cite_start]Gender and Marital Status[cite: 209].
    * [cite_start]Region and Home Ownership[cite: 212].
    * [cite_start]Employment Status and Education Level[cite: 220].
    * [cite_start]Age (Binned) and Has Children[cite: 232].
    * [cite_start]Political Affiliation and Region[cite: 241].

## Key Findings

### Descriptive Analysis Summary

* [cite_start]**Age:** The distribution of age appears to be normal and symmetrical[cite: 251, 174]. The key statistics are:
    * [cite_start]Mean: $43.58$ [cite: 135]
    * [cite_start]Median: $43.00$ [cite: 135]
    * [cite_start]Standard Deviation: $14.919$ [cite: 135]
* [cite_start]**Household Income:** The income range is from a minimum of $\$20,016$ to a maximum of $\$149,997$[cite: 138, 196]. [cite_start]No outliers were found in Household Income[cite: 207, 252].
* [cite_start]**Internet Usage Hours:** The distribution is fairly uniform and very close to being symmetrical[cite: 251, 141, 193].
    * [cite_start]Skewness: $0.014$ [cite: 140]
    * [cite_start]Kurtosis: $-1.191$ [cite: 140]

### Relationship Analysis Summary

[cite_start]The analysis found that many key demographic variables are independent of each other[cite: 252].

| Relationship | Chi-Square ($\chi^2$) Value | Degrees of Freedom (df) | $p$-value | Conclusion (Significance at $\alpha=0.05$) | Source |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Region \* Owns Home** | $3.233$ | $4$ | $.520$ | [cite_start]**Not Significant** [cite: 253, 216] [cite_start]| [cite: 216] |
| **Employment Status \* Education Level** | $15.289$ | $9$ | $.083$ | [cite_start]**Not Significant** [cite: 230, 225] [cite_start]| [cite: 225] |
| **Political Affiliation \* Region** | $15.845$ | $12$ | $.198$ | [cite_start]**Not Significant** [cite: 254, 247] [cite_start]| [cite: 247] |
| **Age (Binned) \* Has Children** | $.411$ | $3$ | $.938$ | [cite_start]**Not Significant** [cite: 236] [cite_start]| [cite: 236] |

[cite_start]The only notable finding regarding the binned age group and children is that the **45-60 age group** has the highest percentage (50.2%) of respondents with children[cite: 239, 255].

## Real-World Applications

[cite_start]The findings provide valuable insights for strategic planning[cite: 256]:

* [cite_start]**Marketing Targeting:** A company selling family-oriented products could focus its marketing efforts on the **45-59 age group**, as this group has the highest percentage of respondents with children[cite: 257].
* [cite_start]**Policy Making:** The lack of a significant relationship between region and homeownership suggests that housing policy initiatives aimed at increasing homeownership should be broad and not solely focused on specific geographical regions[cite: 258, 260].

---
