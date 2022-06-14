# Week 1

## Definition

* Machine learning: without explicit code



## Cost Function

* it is a function of two variables $$θ_1$$ and $$θ_0$$

![the reason that we use 2m: we want to rule out the power 2 for easy calculation](<.gitbook/assets/Screen Shot 2022-06-10 at 2.41.09 PM.png>)

* the function represents **the mean of squared error**



## Gradient Descent Algorithm

* we want to find the minimum of the function J
* it is like we are climbing down the mountain, and alpha $$a$$ is the step we take
* even $$a$$ is fix, the algorithm will **gradually decrease** alpha for convergence
  * small $$a$$: take long time to converge
  * big $$a$$: we may directly jump over the local minimum and "climb up"

![](<.gitbook/assets/Screen Shot 2022-06-10 at 2.59.45 PM.png>)

* the algorithm for some linear regression

![](<.gitbook/assets/Screen Shot 2022-06-10 at 2.43.08 PM.png>)

* note: why $$θ_1$$ will multiple $$x_i$$:
  * we just take derivative of the function h with respect to $$θ_i$$
  * $$h(θ_1,θ_0) = θ_1*x +θ_0$$
  * with respect to $$θ_1$$, x is left, but with respect to $$θ_0$$, x will be seen as a constant
* note: **we will not get stuck in local minimum since for linear regression, we only have one global minimum ---> so it will always converge**&#x20;
* batch gradient descent: we take the mean of the gradient of the training set for determining the next (the one above)



