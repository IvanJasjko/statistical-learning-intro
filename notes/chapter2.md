# Chapter 2

### Statistical Learning

#### 2.1.1

**Input** variables are usually denoted as *X*<sub>n</sub> and are often called *predictors, independent variables, features*. 

**Output** variables are denoted as *Y* and are often called *responses, dependent variables*.

In essence statistical learning is about approaches to estimating  *ƒ* where *Y = ƒ(X) + e* and *e* is a random error term with mean zero.

*ƒ* is estimated for **prediction** and **inference**

#### Prediction

Often output Y can not be obtained, while X is available. If all inputs are available, error term averages at 0 and Y can be predicted using,

 *Y^ = ƒ^(X)* 

Where ^ denotes an estimate for Y and *ƒ*.
Accuracy of Y^ depends on *reducible error* and *irreducible error*.
*ƒ^* improvements (use of other statistical methods) can *reduce* error

Y^ will never be a perfect estimate of Y because perfect *ƒ* does not account for *e* <= *Irreducible error* 

Irreducible error always provides an upper bound for accuracy of the prediction and is almost always unknown.

#### Inference

Understanding the relationship between X and Y

- Which predictors are associated with response?
- Relationships between response and different predictors (positive or negative) ?
- Is relationship linear?



Models are chosen on the basis of prediction vs inference vs both, e.g. linear models allow for high inference but might yield less accurate predictions compared to other models.

#### 2.1.2

Observations (number of data points) is referred to as training data

For statistical learning we need to find *ƒ^* such that Y = *ƒ^*(X) for any observation (X, Y), most learning methods can be *parametric* or *non-parametric*

#### Parametric Methods

A two step model-based approach:

1. Make an assumption about the functional form of *ƒ*
2. *Fit* or *Train* the model. (Most common approach is (ordinary) *least squares*)

Parametric approach reduces the problem to estimating a set of parameters.

The downside of parametric approach is that the model of *ƒ* may not match the actual *ƒ*. We can try to use more flexible models which can fit different functional forms, however that would require estimating more parameters and can lead to overfitting the data. 

Overfitting means data is too vairable/sensitive and is heavily influenced by errors and noise, thus yielding inaccurate predictions.

#### Non-parametric Methods

Non-parametric methods do not assume functional form of *ƒ*. However, they require a very large number of observations in order to estimate *ƒ*.

#### 2.1.3

Linear regression is an example of an *inflexible* approach since it can only generate linear functions ( / ).

However, restrictive (inflexible) models are much easier to interpret (useful for inference)

Usually, there is a trade-off between **Interpretability** and **Flexibility**. 

Highly flexible models also have a high risk of overfitting, this sometimes leads to less flexible models (considered less accurate for prediction) yielding better results.

#### 2.1.4

**Unsupervised Learning** problems have no associated response y<sub>i</sub> for x<sub>i</sub>. One of the methods to address these problems is *clustering*

There also are *semi-suprevised* problems, usually when predictors can be measure cheaply, but responses are expensive to collect.

#### 2.1.5

Categorical variables take values from different classes (A, B, C)

Quantitative variables take numberical values (height, width, etc.)

Statistical methods can be used for either qualitative or quantitative responses.

### 2.2 Assessing Model Accuracy

#### 2.2.1

Most common measure of model accuracy in regression setting is *mean squared error* (MSE)

$$
MSE = \frac{1}{n}\sum_{i=1}^{n}(y_i - f'(x_i))^2
$$
MSE is small for accurate predictions. Training data MSE is not very relevant compared to MSE inferred from testing data e.g. an MSE for x<sub>0</sub> and y<sub>0</sub> where n = 0 refers to previously unseen observation.

*Smallest training data MSE often may not have the lowest test MSE*

**General Rule: As flexibility of the statistical learning method increases, training MSE is decreasing, while test MSE may not decrease (forming a U shape)**

**Overfitting -> small training MSE and large test MSE** (Training MSE is always expected to be smaller, so overfitting occurs when reduction in training MSE yields larger test MSE than it could have been.)

*Cross-validation* - A good method for estimating test MSE from training data.

#### 2.2.2