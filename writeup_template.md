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
1. detecting white colors
2. canny edge detection
3. dilation
4. Hough tranform line detection
5. drawing the lines



### 2. Identify potential shortcomings with your current pipeline


It is having issues with detecting yellow lines as I have used color based filtering initially, which needs to be fixed.

### 3. Suggest possible improvements to your pipeline

A possible improvement would be tuning the color detection section with yellow | white and also gettign intersection of edge detection on originial image and the color filtered image.