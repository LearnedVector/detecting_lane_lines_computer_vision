**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

###1. My pipeline has #6 notable steps to detect lane lines from a picture or video stream. 

    1. Gray scale the image to help filter out noise for edge detection
    2. Do canny edge detection to identify all edges
    3. Find Region of Interests for filter out un-wanted edges
    4. Hough Transform to identify x, y values of each line detected
    5. Average left and right line slopes then extrapolate lane lines
       a. To do this I seperated the right and left lines by identifying the slope of each line (look in draw_lines() method)
    6. Draw in lane lines with thicker weights

![alt text][output/lane_line.png]


###2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


###3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
