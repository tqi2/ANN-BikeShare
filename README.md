# BikeShare-Prediction-with-NeuralNet
Developed as coursework for Udacity Deep Learning Nanodegree. In this project, I built a simple neural network,1 hidden layer with 12 units, sigmoid as activation function, to predict daily bike rental ridership at Washington D.C.

## Dataset & Background
Bike-sharing rental process is highly correlated to the environmental and seasonal settings. For instance, weather conditions, precipitation, day of week, season, hour of the day, etc. can affect the rental behaviors. The core data set is related to the two-year historical log corresponding to years 2011 and 2012 from Capital Bikeshare system, Washington D.C., USA which is publicly available in http://capitalbikeshare.com/system-data. 

## Goal
The Neural network was built from "scratch", using only NumPy without other frameworks like Keras and Pytorch (see *my_answer.py* for the raw NN code). The goal of this project is to understand the neural network algorithm, how to implement it by myself and prepare to dive deeper into TensorFlow and PyTorch.

## Result

After 3000 iterations, the validation loss ends very low with 0.146, the prediction on test data returns a pretty good result.

However, the network is not able to capture the seasonality in the data during Christmas. This might be because of the lack of data for the holiday period. The issue is that there is only one period of Christmas Holidays that the model has encountered during. So, it is not able to figure out if that is an aberration or a pattern. Had the model seen more such holiday periods, it should have been able to figure that out. Augmenting the original data with more data for Christmas holidays should surely help.


