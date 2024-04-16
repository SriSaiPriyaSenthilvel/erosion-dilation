# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.
<br>
### Step2:
Create the Text using cv2.putText
<br>

### Step3:
Create the structuring element
<br>

### Step4:
Erode the image
<br>

### Step5:
Dilate the image
<br>

## Program:

```
Developed by: Sri Sai Priya. S
Register number: 212222240103
```
# Erode the image
```

import numpy as np
import matplotlib.pyplot as plt
import cv2
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'TheAILearner',(5,70),font,2,(255),5,cv2.LINE_AA)
kernel = np.ones((5,5), np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image_erode1=cv2.erode(img1,kernel1)
plt.imshow(image_erode1)
plt.axis('off')
```
# Dilate the image
```
kernel = np.ones((5,5), np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image_dilate1=cv2.dilate(img1,kernel1)
plt.imshow(image_dilate1)
plt.axis('off')
```
## Output:
### Display the Eroded Image

![image](https://github.com/SriSaiPriyaSenthilvel/erosion-dilation/assets/119475702/5618a074-95ca-4d70-80a8-344d3154e965)
<br>

### Display the Dilated Image

![image](https://github.com/SriSaiPriyaSenthilvel/erosion-dilation/assets/119475702/7b01cee5-4078-4552-bff5-a56eb7a4b902)

<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
