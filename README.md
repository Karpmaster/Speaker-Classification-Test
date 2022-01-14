# Speaker-Classification-Test
A small project to test out whether is it the model or dataset causing wrong predictions.

# Project Intro
Originally, I have recorded a audio dataset for a speaker classification project. However, it turned out bad.
The chances of getting wrong prediction is relatively high. So there can be only two possible reasons：
1. Bad model structure.
2. Bad quatity or bad quality dataset.

After some research on another similar audio classification projects, I assume my problem is tend to be a bad dataset.
So, this is small project is to test whether is it the model structure or poor quality data in the dataset casuing the miss prediction.

# Dataset source
Basically, I won't change the model sturcture I originally desinged. But test it with a public dataset.
Public datset source: https://www.kaggle.com/kongaevans/speaker-recognition-dataset

# Details
I designed a CNN model with tensorflow. Using Librosa to extract the MFCC features. And output as a json file.
Split the data in the json file into train, validation, test sets for a cross validation later on.
The pridiction print output includes all similarity percentage of each class. And will choose the highest percentage index.

# Result
Surprisingly, I got really good result getting all the right indexes with the original model structure but with public dataset.
Conclude that it is my dataset causing the problem.
