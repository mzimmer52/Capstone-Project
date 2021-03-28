# Summary

## My capstone project comprised of using selenium to webscrape information from cross-fit athletes around the world, and then ultimately making a model that could predict the ranking of an athlete given their stats/results. 


# Selenium

## The python library, Selenium, was used to help scrape all the relevant data from the tables. Beautiful Soup was not effective in this task, as the table was updated using javascript. In the end, I was able to receive 20,000 rows of data through the use of loops, and automated clicking features. 


# Data Manipulation


<img src="Images/20.1"> <img src="Images/20.3">

## Most of the data seemed to follow a similar trend. As seen from the images above, there is a clear pattern where the athletes ranked higher tend to have better scores for each event. Concering features like weight and height, it was interesting to see how the higher an athlete was ranked, the less their height/weight seemed to differ from the rest of their peers in the same class. 

<img src="Images/Weight"> 

# Models

## In the end, the machine learning model that provided the best accuracy for the dataset was a neural network. I was able to utilize Keras Tuner in order to find the parameters that were best fit to the dataset. 

<img src="Images/Keras_Tuner"> 

## To make sure my local machine did not have to overwork/the session did not time out, the model was run in a Google Collab notebook using Google's GPU.

## In the end, the neural network was able to obtain an accuracy of approximately 85%. The confusion matrix is shown below:

<img src="Images/Matrix"> 

## As we can see, the results are accurate, and are only off by one class on average for every mistaken prediction. 

## Using a decision tree, I was able to see which features in the dataset mattered the most for each prediction.

<img src="Images/importances"> 

## Not surprisingly, the actual results for each event were the most important regarding the prediction to which class an athlete belonged to. The weight, age, and height were not a important.

