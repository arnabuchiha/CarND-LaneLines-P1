# **Finding Lane Lines on the Road** 

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./interms/solidWhiteCurve.jpg "After Edge detection"
[image2]: ./test_images_output/solidWhiteCurve.jpg "After applying Hough lines on original image"
---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of the following steps:

1. Convert RGB images to grayscale
2. Apply Guassian blur on the grayscale image
3. Applied Canny Edge Detector
4. Fix the area of interest of the image
5. Produce the Hough Lines
6. Finally apply the Hough Lines on the original image

![5th step produced the following result][image1]

![6th step produced the following result][image2]

### 2. Identify potential shortcomings with your current pipeline


The pipeline works perfectly on the first two videos but it fails for the third video, one of the reason can be that the third video contains curved lanes.


### 3. Suggest possible improvements to your pipeline

1. Applying deep learning may have some improvement
2. Expressing lines as second degree polynomials
