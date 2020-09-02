# Mathematics for Machine Learning: PCA

### Mean of a dataset

Think about a piece of paper that has a number of eights written on it by hand, and we want to find what the average eight looks like. Each 8 can be split into a 3x3 matrix, and then turned into a 9-dimensional vector. We do this for each example, add up the values and then divide by the number of samples. 
$$
D = \{x_1, ... , x_n\}\\
E[D] = 1/n\sum_{n=1}^nx_n\\
$$
Let's use the example of rolling a die 5 times, what is the expected value?
$$
D^1 = \{1, 2, 3, 4, 6, 6\}\\
E[D^1] = (1 + 2 + 4 + 6 + 6)/5 = 19/5 = 3.8
$$

### Variance and covariance

What other properties can we easily find about a dataset? The mean is describes the center, the variance is the spread of data points around this center and is very useful.
$$
D_1 = \{1, 2, 4, 5\}, E[D_1] = 3\\
D_2 = \{-1, 3, 7\}, E[D_2] = 3\\

D_1 = \frac{(1-3)^2 + (2-3)^2 + (4-3)^2 + (5-3)^2}{4} = 10/4\\
D_1 = \frac{(-1-3)^2 + (3-3)^2 + (7-3)^2}{4} = 32/3\\
X = \{x_1,...,x_n\}\\
Var[X] = 1/n\sum_{n=1}^n(x_n - \mu)^2\\
\mu = E[X]
$$
What about more than one dimension? The variance along 2 or more dimensions is called the covariance.
$$
cov[x,y] = E[(x-\mu_x)(y-\mu_y)]\\
\mu_x = E[x]\\
\mu_y = E[y]\\
var[x]\\
var[y]\\
cov[x,y]\\
cov[y,x]
$$
The covariances of the dataset describe the relationship between x and y, a positive value means that there is a positive correlation between x and y, and a value of 0 means they are uncorrelated.

The variance can be found by:
$$
D = \{x_1,...,x_n\}\\
var[D] = 1/n\sum_{i=1}^n(x_i-\mu)(x_i-\mu)^T
$$

### Linear transformation of datasets

