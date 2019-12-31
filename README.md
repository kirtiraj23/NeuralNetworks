##### NeuralNetworks
Deep Learning 

The design of Artificial Neural Networks (ANNs) is inspired by the animal brain. Although not as powerful as the brain (yet), artificial neural networks are the most powerful learning models in the field of machine learning

the biological neuron works as follows - it receives signals through its dendrites which are either amplified or inhibited as they pass through the axons to the dendrites of other neurons.

Artificial Neural Networks, are a collection of a large number of simple devices called artificial neurons. The network ‘learns’ to conduct certain tasks, such as recognising a cat, by training the neurons to ‘fire’ in a certain way when given a particular input, such as a cat. In other words, the network learns to inhibit or amplify the input signals in order to perform a certain task, such as recognising a cat, speaking a word, identifying a tree etc.  

##### Perceptron

The perceptron takes a weighted sum of multiple inputs (along with a bias) as the cumulative input and applies a step function on the cumulative input, i.e. it returns 1 if the input is positive, else -1. In other words, the perceptron “fires” (returns 1) if the cumulative input is positive and "stays dormant" (returns 0) if the input is negative.

 here one can rather use 1 and -1 as well instead of 1 and 0:

##### y=1 if x>0

##### y=0 if x<=0

the input to a perceptron is the sum of weights multiplied with their respective inputs and the bias:

##### Cumulative Input = w1x1+w2x2+....+wkxk+b

w and x are vectors representing the weights and inputs as follows (note that, by default, a vector is assumed to be a column vector):

![image](https://user-images.githubusercontent.com/16449922/71541682-ca9d1180-2982-11ea-93c9-2f9910ded1d7.png)


More precisely:-
the weighted sum of w  and x is using the dot product of wT and x . The transpose of w  is wT =[w1 w2..wk] - a row vector of size 1xk. Taking the dot product of wT with x:

![image](https://user-images.githubusercontent.com/16449922/71541703-15b72480-2983-11ea-9942-1dc0980082cd.png)

![image](https://user-images.githubusercontent.com/16449922/71541752-c6bdbf00-2983-11ea-8590-5d68a3f1dd5b.png)


##### The 'sign function' is similar to the step function - it outputs +1 when the input is greater than 0 and -1 otherwise. In a binary classification setting, +1 and -1 represent the two classes.


![image](https://user-images.githubusercontent.com/16449922/71620205-a7769a00-2bee-11ea-8d88-e04511c69c62.png)


![image](https://user-images.githubusercontent.com/16449922/71620243-d3921b00-2bee-11ea-80e1-731431f6f49d.png)

where yit.xit
 is the error term. It is important to note here that xit
 in this iterative procedure is a misclassified data point and 
yit is the corresponding true label. Also, note that the dot in yit.xit is not a dot product. 



