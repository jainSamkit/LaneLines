# **Finding Lane Lines on the Road** 

## Writeup Template

---

**Finding Lane Lines on the Road**


### Description of the pipeline.

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I applied gaussian blur with suitable kernel to remove the noise.After blurring ,I applied canny edge detection to detect the edges on the image.I set the high threshold as 150 and subsequently low threshold as 50.Other parameters can be chosen as well.Further,I masked out the irrelevant portions of the image i.e the ones without lane lines.From camera's perpective I only needed to clip a trapezium from the bottom of the frame to focus on the lane lines.After filtering out the ROI,I applied hough tranform to find the set of line segments on it.These line segments together determine the left and right lane lines.

In order to draw a single line on the left and right lanes, I modified the draw_lines() in two ways:
1.

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
