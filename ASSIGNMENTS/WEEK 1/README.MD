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

cap = cv2.VideoCapture(0)

if (cap.isOpened() == False): 
  print("Unable to read camera feed")

frame_width = int(cap.get(3))
frame_height = int(cap.get(4))

out = cv2.VideoWriter('outpy.avi',cv2.VideoWriter_fourcc('M','J','P','G'), 10, (frame_width,frame_height))

while(True):
  ret, frame = cap.read()

  if ret == True: 
  
  else:
    break  

cap.release()
out.release()

cv2.destroyAllWindows()
