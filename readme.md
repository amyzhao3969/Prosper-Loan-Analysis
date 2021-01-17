## Communicate Data Findings
### By Yiming Zhao

## Table of Contents
<ul>
<li><a href="#overview">Overview</a></li>
<li><a href="#eda">Exploratory Data Analysis</a></li>
<li><a href="#ea">Explanatory Analysis</a></li>
<li><a href="#conclusions">Conclusions</a></li>
</ul>

<a id="overview"></a>
### Overview

This data set is from Prosper. It contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others. 

The goal is to understand the effects of borrower and loan attributes on borrower's APR and loan outcomes. To achieve this goal, we will firstly conduct a data wrangling such as handling missing values and transform scales of certain variables. And then we will explore the features by identifying variables, and performing univariate, bivariate, and multivariate analyses. Finally we will polish our findings through different visualizations and make conclusions.

<a id='eda'></a>
### Exploratory Data Analysis

This stage summarizes the main characteristicsc of different variables by using different visualization tools. And then we use the characteristics to suggest hypothese. 

Univariate, bivariate, and multivariate plots are used to explore the relationships in the data set. Through questioning and investigation, interpretations are summarized for explanatory data analysis. 

Through EDA, we assess the assumptions we made about how different factors may potentially impact borrower's APR, and then use the tools mentioned above to support our findings. Through this process, we removed the outliers that may impact the visualization and transform the scale of monthly income and principal amount to have a better understanding of the variables.

#### Summary of Findings during EDA
- When investigating borrower's debt to income ratio, a number of outliers were identified. 99% of the borrower's debt to income ratio is under 1%. For further analysis, the outliers were removed from the dataset.
- The principal variable looks highly skewed in its natural units. Under the transformation, the data looked normally distributed with one peak around 5k.
- Most of the borrowers are employed and full-time workers. Through their occupations, it prove that the borrowers have a stable source of income, such as computer programmer and executives.
- Most of the loan status is under current, which means still in progress. The second biggest chunk of the borrower's status is completed, with only a few charged-off and defaulted loans.
- Borrowers APR, borrowers interest, estimated return are highly correlated with one another. In addition, borrower's rate and credit score are negatively correlated, which means the higher the credit score, the less the borrower's rate.
- There is a negative correlation between borrower's APR and loan original amount. 
- Larger amount of loans usually has lower rate of estimated return.
- The distribution of estimated return is lot higher for low prosper score borrowers with the range from -0.26 to 0.28.
- Among different loan status, borrower's prosper score have a systematic negative impact on the average APR.
- There is a modest positive relationship between monthly income and principal borrowed. 

<a id='ea'></a>
### Explanatory Analysis

This stage summarizes the main findings from EDA process. We polish the visualization, and select only certain representative findings to better communicate our findings.

#### Summary of Findings for Explanatory
- Borrowers APR ranges from almost 0 to 0.5. The distribution of APR takes on a bell shape, with a spike at around 0.35 to 0.36.
- Most of the borrower's monthly income is within the range of 2500 𝑡𝑜 7500, with the distribution skewed to the right. Most of the principal amounts are between  5𝑘− 10k, and the principal is normally distributed, plotted onn a logarithmic scale.
- Borrower's APR, borrower's interest, estimated return, and borrower's credit score are highly correlated with each other.
- As the principal amount increases, the borrower's APR descreases.
- Past due/defaulted/charged off loans happen among various prosper score borrowers, and happen more frequently with the loan term increases.
- There is a roughly positive relationship between monthly income and principal borrowed. 

<a id='conclusions'></a>
### Conclusions
This data set analysis help us understand the factors which impact borrower's APR, and different attributes that affect a loan outcome. At the same time, there are also limitations which may impact our conclusion. For example, in order to have a clearer data visualization, we select a sample instead of using the whole population. The characteristics of the sample may not represent the whole dataset. 


```python

```
