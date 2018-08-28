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

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I call gaussian_blur() function with args kernel_size = 5, then finding out canny edges, then defined vertices for region of interest, then hough lines, and finally calling weighted_img() function 

I did not modeify draw_lines(), but I changed vertices axis value for region of interest. I still don't known why and how to modify draw_lines() function.


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when the Lane Lines is not in the vertices axis value in the images or videos.

Another shortcoming could be the Lane Lines is curve.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to dynamic adjust the vertices axis value.

