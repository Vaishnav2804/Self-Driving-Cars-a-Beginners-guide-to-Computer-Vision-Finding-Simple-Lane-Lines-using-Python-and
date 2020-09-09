# Self-Driving-Cars-Simple-Lane-Lines-using-Python
Essential Computer Vision techniques to identify lane lines on a road.
# OpenCV Installation
You can install OpenCV using pip package installer.
pip install opencv-python

# Lane line detection using OpenCV
# Step 1 Loading the Image Frame and defining the Region of Interest
The purpose of this section is to build a program that can identify lane lines in a picture or a video frame. When we humans drive, we use eyes and common sense to drive. We can easily identify the lanes on the road, and we do the steering based on that. But to do this with machines, it’s a difficult task and that’s when computer vision comes in. We build complex computer vision algorithms in order to teach machines to identify the lane lines.

USE test_image.jpg

# Step 2 Loading this image and converting it into grayscale.

# Step 3 Reduce Noise and Smoothen Image
This image consists of Noise and we need to remove them. Noise can be removed by blurring it. Image Noise creates false edges and can ultimately affect edge detection which is a very crucial step in lane line detection. There could be many reasons for blurring, but here we will use it to reduce the noise. We will use the Gaussian Filter to blur the image. A Gaussian filter nonuniform low pass filter.

# Step 4 Edge Detection (Canny)
Canny Edge detection is one of the widely used Edge Detection Algorithm. Developed by John Canny in 1986, it is a multi-stage algorithm for edge detection. The various stages of Canny Edge Detection algorithm are:
1. Noise Reduction
2. Finding Intensity Gradient of Image
Image for post
Intensity Gradient
3. Non-Maximum Suppression
4. Hysteresis Thresholding
Canny Edge function also implements 5 X 5 Kernel Gaussian Filter that we used in the previous step. Even though Canny has it’s own function for removing noise, it is advised to implement your own Blurring Function before Canny Edge Detection.

# Step 5 Region of Interest
# Step 6 Line Detection — Hough Transform
