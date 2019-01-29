# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.
Following are the steps which my pipeline does
1. detecting white color and yellow color strips with threshold [200,200,100] for RGB respectively
2. Region of interest using polyfit (quadrilateral region)
3. canny edge detection on the color filtered image
4. dilation using kernel of size (8,8)
5. Hough tranform line detection - in hough transform function draw_lines is used.
5. drawing the lines



### 2. Identify potential shortcomings with your current pipeline


The dilation kernel size needs to be tuned, seems there could be a better alternative of dilation.

### 3. Suggest possible improvements to your pipeline

A possible improvement would be tuning the color detection section with yellow | white and also gettign intersection of edge detection on originial image and the color filtered image.
