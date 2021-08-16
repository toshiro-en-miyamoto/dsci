# Chapter 3: Statistics

## Attributes

An attribute is a column or data field or series that represents the characteristics of an object and is also known as a variable, a feature, or a dimension:

- statisticians use the term *variable*
- machine learning engineers prefer the term *feature*
- the term *dimension* is used in data warehousing
- database professionals use the term *attribute*

Types of attributes include:

- *Nominal attributes*: of categorized variables, e.g.product name, brand name, zip code, state, gender, and marital status
- *Ordinal attributes*: of a meaningful order or ranking, but the magnitude of values is not known, e.g. customer satisfaction ratings (e.g., 1: Very dissatisfied, 2: Somewhat dissatisfied, 3: Neutral, 4: Satisfied, 5: Very satisfied), product ratings, and the size of drink (small, medium, or large)
- *Numerical attributes*: of interger or real values, further categorized as:
  - *Interval-scaled attributes*: such as the birth year, and the temperature in °C; such data can add and subtract but can't multiply and divide because of no true zero
  - *Ratio-scaled attributes*: such as height, weight, latitude, longitude, years of experience, and the number of words in a document; we can perform multiplication and division, and calculate the difference between ratio-scaled values

Another way to classify attributes:

- *Discrete variables*: accept only a countable finite number, such as how many students are present in a class, how many cars are sold, and how many books are published. It can be obtained by counting numbers.
- *Continuous variables*: accept an infinite number of possible values, such as the weight and height of students. It can be obtained by measuring.

## Central tendency

The mean value is the arithmetic mean or average. It is sensitive to outliers and noise, with the result that whenever uncommon or unusual values are added to a group, its mean gets deviated from the typical central value.

The median is the midpoint or middle value in a group of observations. It is also called the 50th percentile. The median is less affected by outliers and noise than the mean, and that is why it is considered a more suitable statistic measure for reporting. It is much near to a typical central value.

The mode is the highest-occurring item in a group of observations. The mode value occurs frequently in data and is mostly used for categorical values. If all the values in a group are unique or non-repeated, then there is no mode.

- *mean*: `pandas.Series.mean()`
- *mode*: `pandas.Series.mode()`.
- *median*: `pandas.Series.median()`.

| Attribute | Mode  | Median  | Mean    |
| --------- | ----- | ------- | ------- |
| Nominal   | &cir; | &cross; | &cross; |
| Ordinal   | &cir; | &cir;   | &cross; |
| Numeric   | &cir; | &cir;   | &cir;   |

## Measuring dispersion

The most popular dispersion metrics are

- *range*: `range = pandas.Series.max() - pandas.Series.min()`
- *interquartile range (IQR)*: `iqr = pandas.Series.quantile(.75) - pandas.Series.quantile(.25)`
- *standard deviation*: `sd = pandas.Series.std()`

Note that `pandas.Series.describe()` generates descriptive statistics. For numeric data, the result’s index will include `count`, `mean`, `std`, `min`, `max` as well as (25, 50, 75) percentiles. The 50 percentile is the same as the median.

## Skewness and kurtosis

Skewness measures the symmetry of a distribution. It shows how much the distribution deviates from a normal distribution. Its values can be zero, positive, and negative.

- A zero value represents a perfectly normal shape of a distribution.
- Positive skewness is shown by the tails pointing toward the right—that is, outliers are skewed to the right and data stacked up on the left.
- Negative skewness is shown by the tails pointing toward the left—that is, outliers are skewed to the left and data stacked up on the right.

The skewness of a series can be computed with `pandas.Series.skew()`.

## Covariance and correlation coefficients

Correlation shows how variables are correlated with each other. Correlation offers a better understanding than covariance and is a normalized version of covariance. Correlation ranges from -1 to 1.

- A negative value represents the increase in one variable, causing a decrease in other variables or variables to move in the same direction.
- A positive value represents the increase in one variable, causing an increase in another variable, or a decrease in one variable causes decreases in another variable.
- A zero value means that there is no relationship between the variable or that variables are independent of each other.

Have a look at the following code snippet: `data.corr(method='pearson')`

The `method` parameter can take one of the following three parameters:

- *pearson*: Standard correlation coefficient
- *kendall*: Kendall's tau correlation coefficient
- *spearman*: Spearman's rank correlation coefficient

**Spearman's rank correlation coefficient** is Pearson's correlation coefficient on the ranks of the observations. It is a non-parametric measure for *rank correlation*. It assesses the strength of the association between two ranked variables. Ranked variables are ordinal numbers, arranged in order.

First, we rank the observations and then compute the correlation of ranks. It can apply to both continuous and discrete ordinal variables. When the distribution of data is skewed or an outlier is affected, then Spearman's rank correlation is used instead of Pearson's correlation because it doesn't have any assumptions for data distribution.

**Kendall's rank correlation coefficient** or *Kendall's tau coefficient* is a non-parametric statistic used to measure the association between two ordinal variables. It is a type of rank correlation. It measures the similarity or dissimilarity between two variables. If both the variables are binary, then Pearson's = Spearman's = Kendall's tau. 
