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



Models are chosen on the basis of prediction vs inference vs both. e.g. linear models allow for high inference but might yield less accurate predictions compared to other models.

#### 2.1.2

//TODO