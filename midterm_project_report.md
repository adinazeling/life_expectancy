Introduction
------------

The dataset for our analysis was compiled by the Global Health
Observatory (GHO), a branch of the World Health Organization (WHO). The
repository contains data collected from 2000 to 2015 from 193 countries
about factors relating to life expectancy. These factors include
mortality rates of adults as well as infants and children, economic
factors such as GDP and government health expenditures, disease related
data such as incidence of measles and HIV, and health related variables
such as BMI and alcohol consumption. Our analysis aims to answer the
following questions:

-   Which covariates are most predictive of life expectancy?
-   What modeling method most accurately predicts life expectancy?

The results of analyses such as ours can be used by governments to
direct resources and health care expenditures on the variables that are
most strongly associated with life expectancy in order to improve the
population’s longevity and livelihood.

### Data Cleaning

The original data set has 22 variables and 2938 observations from 193
countries between 2000 and 2015. A correlation matrix was used to assess
the predictors to determine if there were any highly correlated
variables. In order to avoid multicollinearity and to create a more
parsimonious model, highly correlated variables were removed. Among the
variables removed were infant deaths, percentage expenditure, measles,
polio, and thinness for children ages 5 to 9 years. Population was also
removed from the dataset because it is not an appropriate standardized
measurement for life expectancy. Without adjusting population for area
it is not a good comparative measurement. One dichotomous variable in
our dataset that describes development status was recoded into an
integer with groups 0 and 1. Any entries with NAs were omitted. The
final analysis dataset has 15 variables with 1853 observations.

EDA
---

In exploratory data analysis, one of the main goals was to characterize
the relationship of predictors with life expectancy. From the
scatterplot in Figure \_, we were able to conclude that several
predictors potentially have a non-linear relationship with life
expectancy. These predictors include GDP, thinness of children ages
1-19, BMI, total expenditure, diphtheria, HIV/AIDS, adult mortality,
alcohol, and hepatitis B.

![](midterm_project_report_files/figure-markdown_strict/unnamed-chunk-2-1.png)

Model Building
--------------

Conclusions
-----------

Appendix
--------
