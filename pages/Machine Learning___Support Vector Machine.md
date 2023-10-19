tags:: Algorithmics
alias:: SVM, Support Vector Machine

-
- a [[Supervised Learning]] machine learning algorithm that can be used for classification or regression.
- a discriminative classifier
	- it tries to find a decision boundary or **hyperplane** that separates the two classes of data
	- the hyperplane maximizes the ((6530fd93-3af6-420a-a14d-543c68201de5)) between the two classes
- **margin**
  id:: 6530fd93-3af6-420a-a14d-543c68201de5
	- is the distance between the hyperplane and the closest data points of each class
- tries to find the hyperplane that has the largest margin
	- will result in the best possible generalization performance on unseen data
- the geometric interpretation of applying SVM binary classification to one or two dimensional data is as follows:
	- In one dimension, the SVM classifier is a line that separates the two classes of data. The line is chosen such that the distance between the line and the closest data points of each class is maximized.
	- In two dimensions, the SVM classifier is a plane that separates the two classes of data. The plane is chosen such that the distance between the plane and the closest data points of each class is maximized.
- the optimization objectives for training an SVM binary classifier are
	- to maximize the ((6530fd93-3af6-420a-a14d-543c68201de5)) between the two classes
		- the larger the margin, the better the generalization performance of the SVM classifier
	- to minimize the misclassification errors
		- misclassification errors are the number of data points that are misclassified by the SVM
		- the lower the misclassification errors, the better the accuracy of the SVM
- Advantages
	- powerful classifier that can achieve high accuracy
	- versatile classifier that can be used with both linear and non-linear data using the Kernel Trick
	- robust classifier that is not easily affected by noise
- Disadvantages
	- can be computationally expensive to train
	- can be sensitive to the choice of hyperparameters
	- can be difficult to interpret the results of an SVM classifier
-
-
- Further Research
  background-color:: purple
	- Read
		- [Support vector machine - Wikipedia](https://en.wikipedia.org/wiki/Support_vector_machine)
	- Watch
		- {{video https://www.youtube.com/watch?v=_YPScrckx28&pp=ygUTbWwgdHJhaW5pbmcgcHJvY2Vzcw%3D%3D}}
		- {{video https://www.youtube.com/watch?v=efR1C6CvhmE&pp=ygUWc3VwcG9ydCB2ZWN0b3IgbWFjaGluZQ%3D%3D}}
		-