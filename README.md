# **Finding Lane Lines on the Road** 
---


## Overview
---

The Purpose of this project is to detect the lane lines on the road by creating a Pipeline algrothim, So the vehicle will use these lines to be able to steer/control its direction. I will use in this project some computer visions algrothims like **Canny Edgy Detection** and **Hough Transfor**, Create a pipeline algrothim and apply it on some static pictures to detect the output lines, then I will modify the algrothim and apply it on some stream videos in order to have output videos with detected lane lines.


## Project
---

### 1. Desciption of Pipeline

**My pipeline consists of 6 steps as follows:**

    1. Convert detected image into gray scale.

    2. Apply Gaussian Blur filter in order to smooth the image.

    3. Apply Canny Edge Detection on the filtered image with a defined low and high threshold using a 1:2 ratio.

    4. Define a four sided polygon in order to mark our region of interest.
    
    5. Apply the hough transform algorithm on the selected region of interest.
    
    6. Draw the filtered lines on the color image.

**In order to draw a single line on the left and right lanes**:

I modified the draw_lines() function as follows:

    1. 



**The following image defines the output of the pipeline algorithm on 6 different images:**

![alt text](https://github.com/KarimDahawy/Finding-Lane-Lines-on-the-Road/blob/master/test_images/Output.png)

### 2. potential shortcomings

One potential shortcoming would be what would happen when the intensity of the line

Another potential shortcoming is the detection of the curved lines as seen in the challenge video as the filtered lines wasn't stable due to the high slope in lines.



### 3. possible improvements

A possible improvement would be to modify the algorithm to detect the 

Another possible improvement is to use another method to detect curved lines like using curve.fit() 



