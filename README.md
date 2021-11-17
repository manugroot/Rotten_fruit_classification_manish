# Rotten_fruit_classification_manish
This repository is contribution of Manish Reddy Radha Reddy for the project Rotten fruit classification.
In thi sproject our aim is to distinguish the difference between the rotten fruits and the fresh fruits.
The dataset which I used in this model, for model training is taken from the kaggle datasets :https://www.kaggle.com/sriramr/fruits-fresh-and-rotten-for-classification
In this dataset we only have different pictures of rotten and fresh oranges, bananas and apples.


**#In the model which I worked on follows naive approach for image classification using deep learning (CNN)**

# Execution of the model

**Step-1:** Import the required libraries to create the model
import os
import numpy
import pandas
import matplotlib.pyplot
import tensorflow
import keras
import IPython.display 

**Step-2:** 
I took the dataset from kaggle and extracted the dataset file in the Downloads folder and renamed the dataset folder as manish_SD_AI.
The manish_SD_AI folder consists one floder named dataset and the dataset folder consists two floders named as train and test which consissts the images of the rotten and the fresh fruits.

Now in this step get the data and then print the file names present in the train or test folder as the model gets trained according to the file names.
Then,I counted the number of images for each classification and printed the result to have the count of images of one particular classification.

**Step-3:**
**Data Augmentation **

I used the ImageDataGenerator to generate the batches of tensor image data with real-time data augmentation.
Here, I rescaled the images to 1/255 and took 80% of the training data for training the model and the rest 20% for model validation.

**Step-4:**
Training the model.

Here, I created a Convolution neural network with three inner layers.

Compile the model using adam optimizer.

After compiling th model fit the model which starts the training the model with the dataset.
Here, I performed 8 epochs.

**MODEL SUMMARY:**
