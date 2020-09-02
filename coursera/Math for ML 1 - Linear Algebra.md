# Linear Algebra

### What does it solve?

A system of linear equations, specifically price discovery of widgets. How do we find what each category costs?
$$
2a + 3b = 8\\
10a + 1b = 13
$$
Let's turn this into a matrix and 2 vectors to solve it.
$$
\begin{bmatrix}2 & 3\\10 & 1\end{bmatrix}\begin{bmatrix}a\\b\end{bmatrix} = \begin{bmatrix}8\\ 13\end{bmatrix}
$$
Vectors are commutative: $r + s = s + r$

Vectors are associative: $(r + s) + t$ is the same as $r + (s + t)$

Vectors are distributive: $r(P + Q) = rP + rQ$

What is the length of a vector $a_i + b_j = \begin{bmatrix}a\\b\end{bmatrix}$ ? $\begin{vmatrix}r\end{vmatrix} = \sqrt{a^2 + b^2}$

### The Cosine Rule

$c^2 = a^2 + b^2 - 2abcos(\theta)$

$\begin{vmatrix}r-s\end{vmatrix}^2 = \begin{vmatrix}r\end{vmatrix}^2 + \begin{vmatrix}s\end{vmatrix}^2 - 2\begin{vmatrix}r\end{vmatrix}\begin{vmatrix}s\end{vmatrix}cos(\theta)$

$(r-s)\cdot(r-s)=r\cdot r - s \cdot r- s \cdot r - s \cdot s$

​			   $=\begin{vmatrix}r\end{vmatrix}^2-2s\cdot r + \begin{vmatrix}s\end{vmatrix}^2$

