## Multinomial Logistic Regression on MNIST dataset

a) Open the notebook [Multinomial Logistic Regression](https://github.com/tensorchiefs/dl_course/blob/master/notebooks/Multinomial_Logistic_Regression.ipynb).
In this notebook we use multinomial logistic regression to predict the handwritten digits of the MNIST dataset.  
We have 4000 examples with 784 pixelvalues and 10 classes. Run the fist 3 cells and explain the OneHot encodig. In TensorFlow we need to  
use OneHot encodig. 

b) Write the missig TensorFlow code in cell 4 to do a matrix multiplication between x and w and then an addtion of b  
$z=x*w+b$

c) Run the next two cells to store the graph and do a foreward pass of the untrained netword, look at the probability for each class of some examples.

c) Now lets train the model. We use a minibatch size of 128 and use the fist 2400 examples for the training.  
The validation set will be the examples from 2400 to 3000. Write the code to get the loss and the probabilities of your validation set.
Run the last cells to check the perfomace of the model and to get the probability of a random example of the validation set.