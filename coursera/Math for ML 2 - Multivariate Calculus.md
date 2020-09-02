# Mathematics for Machine Learning: Multivariate Calculus

### The Jacobian

This include the first-order partial derivatives of each variable in the function.
$$
J = \begin{bmatrix}\frac{\delta{f}}{\delta{x_1}}...\frac{\delta{f}}{\delta{x_n}}\end{bmatrix}
$$

For a function $$f(x,y,z) 

### The Hessian

This includes the partial derivatives of each variable in the function. If the Det of the Hessian is positive at some point, we know that you are looking at a maximum or a minimum.
$$
f(x,y,z) = x^2yz\\\\
J = [2xyz, x^z, x^2y]\\
H= \begin{bmatrix}
2yz & 2xz & 2xy\\
2xz & 0 & x^2\\
2xy & x^2 & 0
\end{bmatrix}
$$



### Chain Rule

I'll look at a multivariate function and see how we can find a multivariate version of the chain rule.
$$
f(x,y,z)=sin(x)e^{yz^2}\\
x=t-1; y=t^2; z=1/t
$$

$$
\frac{df}{dt}= \frac{\delta f}{\delta x}\frac{dx}{dt} + \frac{\delta f}{\delta y} \frac{dy}{dt}+\frac{\delta f}{\delta z}\frac{dz}{dt}\\
\frac{df}{dt} = cos(t - 1)e
$$

But let's break that down a little
$$
\frac{\delta f}{\delta x} = \begin{bmatrix}\delta f/\delta x_1\\\delta f/\delta x_2\\ \vdots\\ \delta f/ \delta x_n\end{bmatrix} = (J_f)^T\\
\frac{df}{dt} = J_f \frac{dx}{dt}
$$


Let's go back and look at a univariate version of the chain rule
$$
f(x) = 5x\\ x(u) = 1-u\\ u(t) = t^2
$$
So the chain rule gives us $f(t) = 5-5t^2$. Differentiating f with respect to t gives us $\frac{\delta f}{\delta t} = -10t$. The chain rule looks like:
$$
\frac{\delta f}{\delta t} = \frac{\delta f}{\delta x}\frac{\delta x}{\delta u}\frac{d u}{d t}\\
\frac{\delta f}{\delta t} = (s)(-1)(2t) = -10t
$$

### Neural Networks

The simplest possible neural network is one neuron feeding into one other neuron. $a^{(0)}  > a^{(1)}$. More precisely we can write this function as:
$$
a^{(1)} = \sigma(wa^{(0)}+b)
$$
a = "activity", w = "weight", b = "bias", $\sigma$ = "activation function".

Adding complexity, two neurons feeding into one. 
$$
a^{(1)} = \sigma (w_0a_0^{(0)} + w_1a_1^{(0)}+b)
$$
This is generalizable for any number of neurons
$$
a^{(1)} = \sigma((\Sigma_{j=0}^{n}w_ja_{j}^{(0)})+b)
$$



### Taylor series for approximations

Taylor series (or power series) are approximations of continuous functions using combinations of terms of increasing powers of x. A generalized form is 
$$
g(x) = a + bx + cx^2 + dx^3 + \dots
$$
We may describe these approximations in terms of order, the 0th order approximation is $g_0(x) = a$, 1st order approximation is $g_1(x)=a+bx$ and so on.

The nth order power series can be found generally as:
$$
g(x)=\Sigma_{n=0}^{\inf}\frac{1}{n!}f^{(n)}(0)x^n
$$
this works where the function is centered at x=0, so this is actually a Maclaurin series and not a taylor series.

If we want to replicate the exponential function $e^x$ using a taylor series, a series of approximations gives us
$$
e^x = 1+x+\frac{x^2}{2}+\frac{x^3}{6}+\dots\\
e^=\Sigma_{n=0}^{inf}\frac{x^n}{n!}
$$
