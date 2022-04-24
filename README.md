# Pedestrian-Detection-and-Tracking

For Pedestrian Detection

The main objective behind this detection is to devise an algorithm to 
identify and track pedestrians from the eyes of a moving vehicle.
## 2 main steps which will be used are

    1) HOG (Histogram of Oriented Gradients) for detection

In the HOG feature descriptor, the distribution ( histograms ) of 
directions of gradients ( oriented gradients ) are used as features.
HOG calculates the horizontal and vertical component of the 
gradient’s magnitude and direction of each individual pixel and then 
organizes the information into a 9-bin histogram to determine shifts in 
the data. 
The main takeaway that you should get from gradients are that the 
magnitude of the gradient increases wherever there is a sharp 
change in intensity.

    2) Kalman Filter for tracking and prediction

The Kalman filter is a corrective predictor filter. In the tracking system 
objects, this filter looks at an object as it moves, that is, it takes 
information on the state of the object at the precise moment. 
Then, it uses this information to predict where the object is in the next 
frame. The KF is very powerful in several aspects: it supports 
estimates of past, present and even future states and it can do so 
even when the exact nature of the modeled system tracking and 
detection objects.
For this, it takes as input a measurement vector (position in x, in y, 
width and height of the object).
