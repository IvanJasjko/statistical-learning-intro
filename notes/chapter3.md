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

The estimate of standard deviation is known as RSE (*residual standard error*) and can be expressed as:

$$
RSE = \sqrt{RSS/(n - 2)}
$$

In general, sample mean provides a good estimate for a population mean. Therefore least squares line defines regression line coefficient estimates. Sample mean is an **unbiased** estimate of population mean, because an average of sample means for a large number of samples would be equal to population mean.

**Unbiased** estimator does not systematically over or under estimate the parameter. The least squares line holds **unbiasedness** property.

**standard error** of a sample mean measures how accurate is the sample mean compared to the population mean.

*Var(sample\_mean) = SE(sample\_mean)<sup>2</sup> = (mean\_sd)<sup>2</sup> / n*.
 Standard error is the average amount by which sample mean differs from the population mean. Additionally, **standard error shrinks when the number of observations is increased**
 
A 95% C.I. is provided 2 SE's for coefficient estimates. Null hypothesis can be true if 0 is included in the confidence interval for an assessed model coefficient.

*t-statistic = coefficient / standard error*. After obtaining t-statistic **p-value** is taken to assess the hypothesis. Small p-value means that null hypothesis is not confirmed.

### 3.1.3

The quality of linear regression fit is assessed using *residual standard error* (RSE) and *R<sup>2</sup>* statistic.

**RSE** is an estimate of the standard deviation of *e* (An average amount that the response will deviate from true regression line). RSE = sqrt( RSS / (n - 2) ). RSE is considered a measure of the lack of fit. If predictions obtained from the model are close to true outcome RSE will be small.

**R<sup>2</sup> statistic** is an alternative measure of fit. It is the proportion of variance explained (hence it is always between 0 and 1). This gives it an advantage over an absolute value of RSE which may be difficult to interpret. 

R<sup>2</sup> = (TSS - RSS) / TSS = 1 - (RSS / TSS) where TSS is the total sum of squares sum(y<sub>i</sub> - y<sub>mean</sub>)<sup>2</sup>

**TSS measures the total variance in the response Y** , it is the amount of variability in the response before regression is performed. On the other hand, **RSS measures the amount of variability that is left unexplained after regression is performed**. Therefore **TSS - RSS leaves only explained variability**. R<sup>2</sup> measures the proportion of variability in Y that can be explained using X.

Under a simple linear regressions setting squared correlation is identical to R<sup>2</sup> statistic.

### 3.2.1

*Multiple Linear Regression* expands on simple linear regression by adding new slope coefficients to each predictor. Multiple linear regression coefficient estimates have complicated forms and require matrix algebra to represent them. Multiple linear regression can be expressed as:

*y = β<sub>0</sub> + β<sub>1</sub>x<sub>1</sub> + β<sub>2</sub>x<sub>2</sub> + ... + β<sub>n</sub>x<sub>n</sub>*

Additionally, in multiple regression every coefficient represents the effect of a predictor while all other predictors remain fixed.

### 3.2.2

Key multiple linear regression question are:

* Is at least one of the predictors useful?
* Are all predictors useful?
* How well does the model fit the data?
* How accurate is the prediction?

To perform a null hypothesis test on multiple regression we need to compute *F-statistic*

TSS = Σ(y<sub>i</sub> − y<sup>-</sup>)<sup>2</sup> where y<sup>-</sup> denotes mean.

RSS = Σ(y<sub>i</sub> − y<sub>i</sub>^)<sup>2</sup>

F = ((TSS - RSS)/p ) / (RSS/(n - p - 1))

When there is no relationship between response and predictors F-statistic is close to 1, on the other hand if null hypothesis is rejected and there is a relationship F-statistic will be greater than 1.

E{RSS/(n − p − 1)} = σ<sup>2</sup> 

E{(TSS − RSS)/p} = σ<sup>2</sup> if (H<sub>0</sub> true)

Where *p* represents the number of predictors and *n* represents the sample size.

F-statistic can be closer to 1 to reject H<sub>0</sub> for large *n*. However for smaller *n* F-statistic needs to be large in order to establish that there is a dependancy.

F test can also be done on a subset of predictors that excludes *q* predictors. We can modify F test to address it in the following way:

F = ((RSS<sub>0</sub> - RSS)/q ) / (RSS/(n - p - 1))

Where RSS<sub>0</sub> is the residual sum of squares for all variables except that last *q* variables. F statistic and most methods can work for smaller numbers of *p* if *p* is large it may not be possible to fit a multiple linear regression model using least squares.

*Variable Selection* is a problem of determining which predictors are needed to fit the model.


**Note** A general expression of RSE = SQRT(RSS / (n - p - 1)). (n - 2) is used for simple linear regressions as p is always 1 in that case.

//TODO reread final bits of 3.2 and add a few more notes

### 3.3.1


 
 