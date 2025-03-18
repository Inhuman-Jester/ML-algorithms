# Logistic Regression

## Where do we use it?

- used in **Classification** problems _(True/False)_
- modifies linear regression to handle edge cases better
- uses **Sigmoid Function** to squash the edges of linear regression line (modification)
- use of sigmoid results in an **'S'** shaped curve

![Comparing logistic and linear regression](https://machinelearninggeek.com/wp-content/uploads/2020/09/0_LeezUk9jfv6X7DG-.png)

> Thank you Machine learning Geek for this image

## Mathematics behind this

### 1. Sigmoid Function

- gives probability that the the input is 1

  - if p(z) < 0.5 then model predicts 0
  - if p(z) > 0.5 then model predicts 1

- The curve of the functtion has its y intercept = 0.5

- ### mathematically denoted by $ ŷ = \frac{1}{1 + e^{-z}} $
  > here z = w\*x + b for our logistic regression ŷ (prediction)

### 2. Cost function

- ### $J(w, b) = J(ŷ) = - \frac{1}{m} \sum\ \left( y^{(i)} \log(\hat{y}^{(i)}) + (1 - y^{(i)}) \log(1 - \hat{y}^{(i)}) \right) $
