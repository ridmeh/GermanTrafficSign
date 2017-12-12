# German Traffic Sign
## Overview
This is Udacity project submission to demonstrate understanding of CNNs using TensorFlow. We are using German Traffic data set for training, validating and testing.
## Setup
You need to create Udacity AMI in Amazon cloud.
Run Jupyter notebooks
Required TensorFlow/Image Processing libraries
## Run
Main code is in Traffic_Sign_Classifier-TBS.ipynb
Outline of steps for running Training/Testing
1. Load training data set images
2. Review their distribution and other aspects to help choose pre-processing/processing parameters
3. Make necessary pre-processing decisions
4. Configure LeNet with decided parameters
5. Train
6. Validate
7. Test
8. Take images from web and check on accuracy 
9. Top K hits

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

