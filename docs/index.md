<head>
<style>
table, th, td {
    border: 0.5px solid black;
    vertical-align: top;
}
</style>
</head>

# Deep Learning (CAS machine intelligence) 

This course in deep learning focuses on practical aspects of deep learning. 

For the hands-on part we provide a docker container ([details and installation instruction](docker.md)).

## Other resources
We took inspiration (and sometimes slides / figures) from the following resources.

* Deep Learning Book (DL-Book) [http://www.deeplearningbook.org/](http://www.deeplearningbook.org/). This is a quite comprehensive book which goes far beyond the scope of this course.

* Convolutional Neural Networks for Visual Recognition [http://cs231n.stanford.edu/](http://cs231n.stanford.edu/), has additional material and videos of lectures. While the focus is on computer vision, it also treats other topics such as optimization, RNNs. Interesting are  the lecture notes which can be found at [http://cs231n.github.io/](http://cs231n.github.io/).


## Syllabus (subject to change)
The course is split in 8 sessions, each 4 hours long. 


<table>
  <tbody>
    <tr>
      <th align="left">Day</th>
      <th align="left">Topic</th>
      <th align="right">Additional Material</th>
      <th align="right">Exercises and homework</th>
    </tr>
    
    <tr>
      <td>1</td>
      <td> 
      		<b>Deep learning basics</b> <a href="https://www.dropbox.com/s/bvgd0wsp0zkgjm0/lecture01.pdf?dl=1">slides</a>
      		<ul>
      			<li>Overview of deep learning</li>
      			<li>Computational graphs, feeding and fetching</li>
      			<li>Loss function (crossentropy)</li>
      			<li>Gradient descent and generalizations</li>
      			<li>Example: linear regression</li>
      		</ul>
      </td>
      <td> 
        Nature review article<a href='http://www.nature.com/nature/journal/v521/n7553/full/nature14539.html'>(LeCun, Bengio, Hinton, 2015)</a>
        DL-book chapter 6
      </td>
      <td>
      	<ul>
      		<li>
      			<a href='https://github.com/oduerr/dl_tutorial/blob/master/tensorflow/linear_regression/01_LineFit.ipynb'> 01_LineFit.ipynb</a> 
      		</li>
      		<li>
      			<a href='https://github.com/oduerr/dl_tutorial/blob/master/tensorflow/simple_ops/ Mandelbrot.ipynb'> Mandelbrot.ipynb</a> 
      		</li> 
      		<li>
      			<a href='https://github.com/oduerr/dl_tutorial/blob/master/tensorflow/stored_models/Loading_Frozen_Graph.ipynb'> Loading_Frozen_Graph.ipynb (Artstyle Transfer)</a> 
      		</li>
         </ul>
      </td>
    </tr>

    <tr>
      <td>2</td>
      <td> 
      		<b>Fully connected networks</b> <a href="https://www.dropbox.com/s/qmfh1ib3dzr50z5/lecture02.pdf?dl=1">slides</a>
      		<ul>
      			<li>Logistic regression</li>
      			<li>Multinomial Logistic Regression</li>
      			<li>Fully Connected networks</li>
      			<li>Regularization:
      				<ul>
      					<li>Early stopping</li>
      					<li>L2 (Weight Decay)</li>
      					<li>Dropout</li>
      				</ul>
      			</li>
      		</ul>
      </td>
      <td> 
      		DL-book chapter 6,7
      </td>
      <td>
      	<ul>
      		<li>
      			<a href='http://playground.tensorflow.org/#activation=sigmoid&batchSize=10&dataset=gauss&regDataset=reg-plane&learningRate=0.1&regularizationRate=0&noise=50&networkShape=&seed=0.01840&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false&stepButton_hide=false&activation_hide=true&problem_hide=true&noise_hide=false&batchSize_hide=true&dataset_hide=true&regularization_hide=true&playButton_hide=false&learningRate_hide=false&regularizationRate_hide=true&percTrainData_hide=true&numHiddenLayers_hide=true'> TF-playground: logistic regression</a> 
      		</li>
      		<li>
      			<a href='https://github.com/oduerr/dl_tutorial/blob/master/tensorflow/path_to_fc_nets/log_reg_challenger.ipynb'> log_reg_challenger.ipynb</a> 
      		</li> 
      		<li>
      			<a href='https://github.com/oduerr/dl_tutorial/blob/master/tensorflow/path_to_fc_nets/Multinomial%20Logistic%20Regression.ipynb'> Multinomial Logistic Regression.ipynb </a> 
      		</li>
      		<li>
      			<a href='http://playground.tensorflow.org/#activation=sigmoid&batchSize=10&dataset=xor&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=5&networkShape=&seed=0.07296&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false&problem_hide=true&batchSize_hide=true&dataset_hide=true&percTrainData_hide=true&regularizationRate_hide=true&learningRate_hide=true&discretize_hide=true&activation_hide=true&regularization_hide=true
'> TF-playground: linear decision boundary</a> 
      		</li>
      		<li>
      			<a href='http://playground.tensorflow.org/#activation=tanh&batchSize=10&dataset=circle&regDataset=reg-plane&learningRate=0.03&regularizationRate=0&noise=0&networkShape=2&seed=0.83173&showTestData=false&discretize=false&percTrainData=50&x=true&y=true&xTimesY=false&xSquared=false&ySquared=false&cosX=false&sinX=false&cosY=false&sinY=false&collectStats=false&problem=classification&initZero=false&hideText=false&showTestData_hide=true&activation_hide=true&problem_hide=true&noise_hide=true&batchSize_hide=true&dataset_hide=true&regularization_hide=true&discretize_hide=true&numHiddenLayers_hide=true
'> TF-playground: universal function approximator</a> 
      		</li>
      		<li>
      			<a href='https://github.com/oduerr/dl_tutorial/blob/master/tensorflow/path_to_fc_nets/fcn_MNIST.ipynb'> fcn_MNIST.ipynb </a> 
      		</li>
      		<li>
      			<a href='https://github.com/oduerr/dl_tutorial/blob/master/tensorflow/path_to_fc_nets/fc_MNIST_keras.ipynb'> fc_MNIST_keras.ipynb </a> 
      		</li>
            </ul>
      </td>
    </tr>





  </tbody>
</table>





