Group Members: Satya Nayak, Ramjee Ganti, Gourav Pattanaik, Jayant Ojha

Scenario 1: 

Objective : Use 15 epocs and reduce number of Parameters to less than 10000

Result : 

Parameters Used : 9,468

Best Train Accuracy : 99.00%

Best Test Accuracy :99.37%

Observation : 

1.	Number of parameters #9648, which is as per the requirement
2.  Current model accuracy  99.37%. But our requirement is 99.4%
3.	Commented out the third convolution layer
4.  Started the network with 8 kernels with gradually increasing
5.  In 2nd convolution layer reduced the kernel size to 10 
6.  Seems to be Good model as testing accuracy is more than training accuracy, however there is a scope to improve the model 

Scenario 2 : 

Objective : Try tranformation functions to see if accuracy changes 

Result 

Parameters Used : 9,468

Best Train Accuracy : 98.92%

Best Test Accuracy : 99.40%

Observation : 

1. Applied ColorJitter with RandomRotation (0.8) transformations 
2. The model reach 99.4% test accuracy only once.
3. Not very consistant.
4. Little more fine tuning required

Scenario 3:

Objective : Decrease dropouts

Result

Parameters Used :9,468

Best Train Accuracy : 99.00%

Best Test Accuracy : 99.43% (Average Test Accuracy 99.26%)

Observation : 

1. Since the model was not overfitting, hence tried reducing the dropouts to 0.8
2. Model accuracy reached to 99.43 but not very consistant
3. It's like the previous result without changing the dropouts.

Scenario 4:

Objective : Increase learning Rate

Result
 
Parameters Used : 9,468
Best Train Accuracy : 99.00%
Best Test Accuracy :99.38%

Observation : 

1. After increasing learning rate to 0.015, there is no change in the accuracy
2. Will try increasing the step size to see if any impact in accuracy in the next run.

Scenario 5: 

Obective : Increase Step size

Result : 

Parameters Used : 9,468

Best Train Accuracy : 98.97%

Best Test Accuracy :99.48%

Observation : 
1. After changing the step size from 6 to 7, the testing accuracy reaches 99.48.
2. Seems step size works!! 