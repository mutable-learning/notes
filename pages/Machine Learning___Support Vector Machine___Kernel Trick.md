tags:: Algorithmics
alias:: Kernel Trick, Kernel Function

-
- used by a [[Support Vector Machine]] to classify non-linear data
- if we have a set of one-dimensional data that is not linearly separable
	- we cannot draw a line that will perfectly separate the two classes of data
- create higher dimensional data by using a kernel function
	- a mathematical function that maps the data points into a higher dimensional space where they can then be linearly separated
- a common kernel function is the polynomial kernel, defined below
	- $K(x, y) = (x · y + 1)^d$
	- where x and y are two data points, and d is a parameter that controls the degree of the polynomial
	- here we use a polynomial kernel with a degree of 2 allowing us to map the data points into a three-dimensional space
	- ![Kernal Trick](https://i.stack.imgur.com/1gvce.png)
	- the data points are now linearly separable in the three-dimensional space
		- we can draw a plane that will perfectly separate the two classes of data
	- the SVM can now be used to classify the data points in the three-dimensional space
	- itwill find the plane that has the largest margin between the two classes of data
- other examples of kernel functions are
	- Gaussian kernel
	- Radial basis function (RBF) kernel
	- Sigmoid kernel
- the choice of kernel function depends on the specific dataset and the problem that is being solved.
-
- Further Research
  background-color:: purple
	- Read
		- [The Kernel Trick in Support Vector Classification | by Drew Wilimitis | Towards Data Science](https://towardsdatascience.com/the-kernel-trick-c98cdbcaeb3f)
		- [Kernel method - Wikipedia](https://en.wikipedia.org/wiki/Kernel_method#Mathematics:_the_kernel_trick)
	- Watch
		- {{video https://www.youtube.com/watch?v=Q7vT0--5VII&pp=ygUMa2VybmVsIHRyaWNr}}