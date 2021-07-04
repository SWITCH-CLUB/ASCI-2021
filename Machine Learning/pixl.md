## Project Name
--------
PIXL

## Domain
---------
Machine Learning
## Link
---------
https://github.com/jijnasu/PIXL

## About Project
--------------------
Our project PIXL recognizes Gun using Deep Learning.

Tech Stack- Python, VS code

## Progress::
-----------------------
week 1:

● we collected data for training and testing dataset\
● we resized the data\
● and processed the images

week 2:

● we labelled each data with their corresponding values\
● we wrote the model for logistic regression\
● and finally by passing training and testing dataset we calculated its accuracy

week 3:

● we made a program to divide a given video into frames to feed our model\
● we made a program that will send email alerts to given email ids if the condition satisfies\
● and finally we integrated all the functions and modules together

## Reference ::
------------
1. DeepLearning.ai (coursera) https://deeplearing.ai
2. geeksforgeeks
3. numpy, pandas and cv2 cheatsheets
4. youtube videos when we encounter any problem 
5. Google images for training and testing dataset

## Team Members
----------------------------
 1. Jyotikrishna Behera
 2. Kumar Jijnasu



# Main Files to run

Processing_data.ipynb :- contains the training and testing dataset which are used to train the model , here the image is resized and labelled to corresponding value of 0 and 1

Model_runner.ipynb :- here we have the logistic regression model with all the calculative functions like sigmoid , cost , gradient descent 

Detect_gun.ipynb :- here we give a video as input and get whether gun is their or not in video, and it contains the email alert program