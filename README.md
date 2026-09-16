# Feature-Distribution and Skewness-Analysis
A technical learning project exploring the Olist dataset through descriptive statistics, feature distributions, skewness, kurtosis, and data transformations. My goal is to understand how data distributions can affect analysis and how to make informed preprocessing decisions.

## About

The main goal of this technical learning project is to understand how descriptive statistics can be used to explore and prepare real-world data for analysis and machine learning.

I want to see how concepts like mean, variance, skewness, kurtosis, and data transformations work on actual data rather than only in theory.

For this project, I’ll be using the **Olist Brazilian E-Commerce dataset** to:

* calculate descriptive statistics
* examine numerical feature distributions
* identify highly skewed features
* visualize the distributions
* apply transformations where appropriate
* compare the data before and after transformation

### Tools

* Python
* Pandas
* NumPy
* Matplotlib
 
# Key Takeaways

- *Descriptive statistics* provide different perspectives on the same feature, helping me understand its typical value, spread, and distribution.

- *Mean and median* can reveal useful patterns in the data. In this dataset, the mean was higher than the median for both `price` and `freight_value`, which aligned with their right-skewed distributions.

- *Skewness* tells me about the direction and degree of asymmetry in a distribution. `price` had a skewness of *7.92*, while `freight_value` had a skewness of *5.64*, showing substantial positive skew.

- *Visualization* is important because the skewness value alone does not show me what the distribution actually looks like.

- I checked the values in each feature before choosing a transformation. `price` contained no zeros, while `freight_value` contained *383 zeros*, which mattered when deciding which transformation to use.

- *Transformations* such as `log1p` and *Yeo-Johnson* can change how a feature is represented and may reduce skewness, but they should not be applied automatically just because a feature is skewed.

- The choice to transform a feature depends on *what the feature represents, the values it contains, the model being considered, and whether the transformation improves the representation of the data*.

- This helped me see descriptive statistics as more than numbers to calculate. They can guide decisions about how to inspect and prepare data before modeling.

## Final Takeaway

I understood that rather than rushing to transform skewed data, the modelling context should come first before deciding whether transformation is appropriate.
