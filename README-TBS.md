# German Traffic Sign
## Overview
This is Udacity project submission to demonstrate understanding of CNNs using TensorFlow. We are using German Traffic data set for training, validating and testing.

## Setup
You need to create Udacity AMI in Amazon cloud.
Run Jupyter notebooks
Required TensorFlow/Image Processing libraries

## Outline of steps performed:
Main code is in Traffic_Sign_Classifier-TBS.ipynb
Outline of steps for running Training/Testing
1. Load training data set images
2. Data Analysis : Review their distribution and other aspects to help choose pre-processing/processing parameters
3. Make necessary pre-processing decisions
4. Architecture: Configure LeNet with decided parameters
5. Train
6. Validate
7. Test
8. Take images from web and check on accuracy 
9. Top K hits

Below are some points explained in more detail :

## 2. Data analysis
Randomly reading some sample images and displaying to see their integrity and get the feel of data that we are dealing. 
After plotting the data distribution of training and test set it becomes clear it is skewed. I am not sure how to mitigate this. If data is not well distributed it could lead to overfitting and high accuracy in training but low accuracy in real world scenarios. For e.g. less number of road specific road sign, could lead to poor classification in real world. Resolution: We could fake data for the signposts that are low in number or reduce the numbers of signposts which are skewing the distribution.
![picture](distribution.png)


## 4. Architecture


## 7. Test with images on web
![picture](5sampleimages.png)

## Observations
1. After certain EPOCHs run, accuracy reaches platue and may start decreasing
2. Distribution of classified images was not good, which created bias in the CNN.
3. Top K gives a real good insight on what CNN has learnt and classifies. 


## Challanges
Based on my current understanding I am ranking the challanges CNN faces
1. Gathering clean, well distributed among (for output classes) normalized data set is the first starting point.
2. Architecture selection or modificaiton for CNN are relatively made easier with TensorFlow. However, understanding all parameters that TensorFlow needs is not easy
3. Running Real-world tests. Always fun but challenging with new inputs. Looking forward to work on continous feedback loop to adjust weights.
4. Need to figure out how to use Top K information to better train CNN

