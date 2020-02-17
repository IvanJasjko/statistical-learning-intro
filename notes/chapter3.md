# Chapter 3

### Linear Regression

### 3.1.1

*Simple Linear Regression* is an approach for predicting the quantitative response *Y* on the basis of a single predictor *X* under a linear relationship assumption.

The most common approach of obtaining model coefficients (intercept and slope of a line) is *least squares*.

For *y^<sub>i</sub> = a^x<sub>i</sub> + b^* (prediction for i<sup>th</sup> value of x) *e<sub>i</sub> = y<sub>i</sub> - y^<sub>i</sub>* (i<sup>th</sup> residual)

RSS = e<sub>1</sub><sup>2</sup> + e<sub>2</sub><sup>2</sup> + e<sub>3</sub><sup>2</sup> + ... + e<sub>n</sub><sup>2</sup> (Residual sum of squares)

It can be written as (*y<sub>1</sub> - a^x<sub>1</sub> - b^*)<sup>2</sup> + ... + (*y<sub>n</sub> - a^x<sub>n</sub> - b^*)<sup>2</sup> => Least squares approach chooses *a* and *b* for which RSS is the smallest.

### 3.1.2

For linear regression (Y = ax + b + *e*) *e* represents the error term and is typically assumed to be independent of x. It is also a *population regression line* which is the best linear approximation to the true relationship between x and y.

The estimate of standard deviation is known as RSE (*residual standard errror*) and can be expressed as:
$$
RSE = \sqrt{RSS/(n - 2)}
$$
