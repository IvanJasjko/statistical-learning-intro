#### 1.

- **A** For an extremely large sample size and a small number of predictors a flexible method would generally yield better results, since larger sample size allows for more flexibility without overfitting and a small number of predictors will result in smaller variance and higher bias, therefore a flexible approach with less bias would be preferred.
- **B** Large number of predictors will reduce bias but greatly increase variance leading to a high chance of overfitting when using a more flexible model. Furthermore, a small number of observations will exacerbate overfitting as there may not be enough data to train a flexible method.
- **C** A highly non-linear relationship can not be modelled by an inflexible method which provides a linear relationship model, therefore a flexible method would yield better results.
- **D** Extremely high variance of error terms will make flexible models with higher variance more prone to overfitting and accounting for noise in training data, therefore a low-variance inflexible approach would yield better results.

#### 2.

- **A** *n* = 500, *p* = 3, Inference, regression problem
- **B** *n* = 20, *p* = 13, Prediction, classification problem
- **C** *n* = 52, *p* = 3, Prediction, regression problem 

#### 3.

- **B** Test error is U shaped becasue larger flexibility leads to overfitting the data and producing incorrect results. Bayes error is a fixed straight line since this error can not be reduced. Training error and bias are always decreasing with increased flexibility since more data points are being accounted for, while bias is decreasing.

#### 4.

- **A** 

  Spam filtering (predictors: number of keywords often occuring in spam messages. response: spam or not spam. prediction)

  Labelling music genres (predictors: instruments used and BPM. response: specific genre. inference). 

  Diagnosing an ilness (predictors: number of symptons. response: specific ilness. prediction) 

- **B** 

  Time to avoid traffic (predictors: number of cars. response: time. prediction)

  Share price (predictors: change in revenue, costs, number of workers. response: share price. prediction)

  Effectiveness of online Ads (predictors: time, content type, userbase size. response: reach. inference )

- **C**

  Identifying new social media trends

  Looking for fraudulent activity

  Discovering target groups for marketing purposes

#### 5.

Flexible approach is preferred when there is a large number of observations and a relatively small number of predictors. Large number of observations will allow for greater flexibility and therefore a less biased approach to the relationship between predictors and response, while lower number of predictors will generate less noise and mitigate overfitting. However a less flexible approach will generally provide better results for noisy data with a large number of predictors. Additionally, smaller sample size might not be sufficient to provide a good estimate when using a flexible model with higher variance.

#### 6.

Parametric approach reduces the problem to estimating a set of parameters, this approach assumes the functional form of the relationship between predictors and response. Parametric approach would yield better results for smaller sample sizes, however this approach can yield inaccurate results if functional form is wrongly estimated. Non-parametric methods can yield more accurate predictions by being more flexible through assuming a functional form. However, non-parametric methods require much larger sample sizes and are more prone to overfitting.	

#### 7. 

- **A**

  1. 3

  2. 2

  3. 3.2

  4. 2.2

  5. 1.4

  6. 1.7

- **B** Green as it is the closest point to required observation.

- **C** Red as 2 out for 3 closest poitns are Red.

- **D** For the non-linear boundary smaller values of K would yield better results as it  smaller K provides more flexibility needed to estimate non-linear relationships.

