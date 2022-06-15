# Week 2

## Multivariate Linear Regression

![](<.gitbook/assets/Screen Shot 2022-06-14 at 2.35.03 PM.png>)

* for convenience, x\_0 is set to 1

![](<.gitbook/assets/Screen Shot 2022-06-14 at 2.47.34 PM.png>)



## Gradient Descent in Practice I

* we use it to **speed up gradient descent ---> each value has the same range**
  * **\*feature scaling\***: rescales the feature so that **-1<= x\_i <= 1**
    * **divided x\_i by range**
  * **\*mean normalization\***: make the **mean of the input = 0** ---> the numerator will be 0
    * ![](<.gitbook/assets/Screen Shot 2022-06-14 at 3.20.36 PM.png>)
    * s\_i can either be **range or standard deviation**
    * **normal distribution**
  *



## Gradient Descent in Practice II - Learning Rate

* learning rate: the alpha
* goal: decrease the cost function value **each iteration**
* too big alpha: cost function **may not decrease on each iteration ---> diverges**
  * if there is cycle like sin(x) ---> divergence
* too small alpha: may take a **long time** to converge
* convergence: when in one iteration **the decrease amount of cost function < a constant** (e.g. 10^-3).



## Features and Polynomial Regression

* we can combine features into a feature
* note **feature scaling**
  * e.g. ft and ft^2



## Normal Equation

![](<.gitbook/assets/Screen Shot 2022-06-15 at 11.22.36 AM.png>)

* X: matrix, y: vector
* we just apply some simple linear algebra knowledge to minimize the cost function
* **no need for feature scaling**

![](<.gitbook/assets/Screen Shot 2022-06-15 at 11.24.19 AM.png>)

* if n > **10000**: we go to iterative
* if (X^T\*T) is not invertible:
  * **linear dependent** ---> singular matrix
  * **too many features**: feature >= data
    * delete features / use regularization
    *
