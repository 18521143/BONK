# 1. Setup Environment
## Create GitHub Repo
[Github Repo](https://github.com/18520877/BONK.git)
## Install Ubuntu desktop
[Ubuntu desktop](https://ubuntu.com/download/desktop)
## Install Python 3.6 or later
[Python 3.9.2](https://www.python.org/downloads/)
## Install OpenCV-Python Package
[OpenCV-Python](https://pypi.org/project/opencv-python/)
# 2. Write a “Hello world” app
## Read, Write and Display a video/webcam using OpenCV python

import cv2
import numpy as np


cap = cv2.VideoCapture('chaplin.mp4')

if (cap.isOpened()== False): 
  print("Error opening video stream or file")

while(cap.isOpened()):
  ret, frame = cap.read()
  if ret == True:
  else: 
    break
    
cap.release()

cv2.destroyAllWindows()
