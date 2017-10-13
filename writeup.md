# **Finding Lane Lines on the Road** 

The project provides a complete understanding of the basic steps needed to perform lane detection.

## Reflection

###  1. Pipeline Summary
1. Convert the image to grey scale. 
2. Perform Gaussian smoothing to blur the grey scale image and remove noise.
3. Run Canny edge detection to obtain the edges.
4. Target the region of the image which consists of lane markings.
5. Perform Hough Transformation to extract lanes from the edges.

#### 1.1 Connect Lines
1. Compute the slopes of the lines after Hough Transforms.
2. Filter out the lines whose slopes |m| < 0.5 as they do not represent a lane.
3. Group the filtered slopes into positive and negative and find the average.
4. Compute the y intercepts
5. Compute the x and y coordinates
6. Draw the lines on the image/video stream


### 2. Identify potential shortcomings with your current pipeline
1. Curved lanes are not detected accurately.

### 3. Suggest possible improvements to your pipeline
1. A non-linear lane detection mechanism.


