tags:: Algorithmics
topic:: [[Algorithm Analysis]]
algo:: Unit 4 Outcome 1

-
- $$
  \begin{align}
  T(n) = \begin{cases}
   a\ \cdot\ T(\frac n b)\ +\ kn^c &\text{if } n>1 \\
   d &\text{if } n=1
  \end{cases}
  \\
  \text{where } a>0,\ b>1,\ c\ge0,\ d\ge0,\ k>0
  \\
  \text{and its solution: } T(n) = \begin{cases}
   O(n^c)\ &\text{if } a<b^c\\
   O(n^c\log(n))\ &\text{if }a=b^c\\
   O(n^{\log_b(a)}) &\text{if }a>b^c
  \end{cases}
  \end{align}
  $$
	-
	- $n$ is the original size of the problem
	- $a$ is the number of recursive calls in the algorithm
	- $b$ is the number of subdivisions of the input data each recursive call makes
	- $c$ is a constant that depends on the algorithm being examined
	- $k$ is the degree (order of degree) of the polynomial defining the work done outside the recursion
- if $a < b^c$ operations are decreasing geometrically and the top level of the recursion requires the most work
- if $a = b^c$ operations are done equally at each level of recursion and the number of levels is the most important aspect
- if $a > b^c$ operations are increasing geometrically and the base case requires the most work to be done
- Increasing or decreasing geometrically is talking about the growth rate as our input moves towards $\infin$
	- increasing geometrically means that the amount of growth increases over time, resulting in a much larger increase in the long run
	- decreasing geometrically means that that the amount of growth is reducing over time
- You can also represent the master theorem as below, and this might be easier to use in practice
	- $$
	  \begin{align}
	  T(n) = \begin{cases}
	     a\ \cdot\ T(\frac n b)\ +\ f(n^k) &\text{if } n>1 \\
	     d &\text{if } n=1
	  \end{cases}
	  \\
	  \text{where } a>0,\ b>1,\ d\ge0,\ k\ge0
	  \\
	  \text{and its solution: } T(n) = \begin{cases}
	     O(n^k)\ &\text{if } a<b^k\\
	     O(n^k\log(n))\ &\text{if }a=b^k\\
	     O(n^{\log_b(a)}) &\text{if }a>b^k
	  \end{cases}
	  \end{align}
	  $$