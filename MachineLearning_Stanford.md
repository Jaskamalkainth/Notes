### Lecture 1:
Introduction to Machine Learning.
#####  Machine learning definition:
> Field of study that gives computers the ability to learn without being explicitly programmed - Arthur Samuel.

Checkers program using ML written by Arthur played better than he did.
> A computer program is said to learn from experience E w.r.t some task T and some performance measure P, if its performance on T, as measured by P, improves with experience E. - Tom Mitchell.


Ex: E: Experience of playing checker game
    T: Playing checker program.
    P: fraction of checker games won
    So with E, P improves on T.

Handwriting Recognition is one the application of ML.
Apply learning algorithms to solve various problems. We use learning algorithms in our daily lifes without even knowing it.
Prerequisits for ML:
Big O notation, Stack, queue, basic programming in MATLAB or octave, Probablity and statistics, Linear Algebra- Eigen value, Eigen vector, Matrix multiplication.


##### Supervised learning

Price($) vs House size (feet^2) Dataset.
we are giving the algorithm this dataset (which is correct) and then we expect machine to learn for future queries.

###### Regression problem: 
Variable we are trying to predict is continous.
###### Classification problem: 
Variable we are trying to predict is discrete values. Ex: A tumor is malignant or benign [0 or 1], depending on the tumor size.

There can be more than one feature using which we devise our learning algorithm.
Our data can lie in 2,3.. n or even infinit dimensional space (IDS)
SVM(support vector machines) maps data to IDS with infinite number of features. [details later].

##### Learning Theory:

learning algorithm for reading zip-codes?
How much training data we need for our learning algorithm?
Tools of ML , use them and apply in solving real life problems.

##### Unsupervised learning

Finding a strucure in a given dataset. *Clustering* is one example of Unsupervised learning algorithm.
Ex: Using clustring algotithm to make 3D model of a 2D image. - Mixture of both type of learning but clustering was the first step.
Ex: Cocktail party problem:
separate out the voice of person of interest in lots of noice.
[*Independent component analysis* (ICA)]
How complicated it is to code?  - 1 line in MATLAB (LOL)

##### Reinforcement learning

In this we make sequence of decisions unlike in supervised learning we say that the cancer is either malignant or benign.

Ex: Make a sequence of good decisions to fly a helicopter.
everytime helicopter crashes, we say bad helicopter. othertime, good helicopter. :P So in the end we need to maximize good helicopter cases.






### Lecture 2:


Given a dataset for Housing price vs house size (training set).
Using this , we need to devise a algorithm to predict housing price for test dataset.
m = #training examples
x = "input" variables / features
y = "output" variable/ "target" variable
(x,y) is one training example (1 row in our data set)

Training set --> Learning algorithm --> hypothesis "h" 
Using "h", we can do this.
 New living area (x) ---> h ---> estimated price (y)
 
 Now a lil Math which is explained here.
 http://cs229.stanford.edu/notes/cs229-notes1.pdf

Learning algorithm computes "Theta's" with which we can compute h(x).
Choose theta's such that the cost funtion is minimized. where cost function is sum of square error.

Now, Use Gradient descent algorithm, which starts with some initial θ, and repeatedly performs the update to minimize the cost function.
With different initial guess of theta we can get a different local minima. [issue].
alpha[learning rate] in the equation is the size of the step you take to compute the next value. So it shouldn't be huge or very small. 

In Batch gradient descent, summation can be computationally expensive when m is in order of millions.
therfore we have, Stochastic Gradient Descent which might not converge to a global minima but to which it converges is a good approximation of a minimum and also this is relatively faster with huge datasets.


Matrix derivatives:




**To be continued.....**







