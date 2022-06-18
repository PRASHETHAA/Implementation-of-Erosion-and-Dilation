# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:

Import the necessary packages.

### Step2:

Create the Text using cv2.putText.

### Step3:

Create the structuring element.

### Step4:

Erode and Dilate the image.

### Step5:

End Program.

 
## Program:
Developed by:Prashethaa R
Register No:212220230036
``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Load the image
img1=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL

# Create the Text using cv2.putText
cv2.putText(img1,' PRASHE ',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img1,cmap='gray')

# Create the structuring element
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))

# Erode the image
img_erode=cv2.erode(img1,kernel1)
plt.imshow(img_erode,cmap='gray')

# Dilate the image
img_dilate=cv2.dilate(img1,kernel1)
plt.imshow(img_dilate,cmap='gray')

```
## Output:

### Display the input Image

![A1](https://user-images.githubusercontent.com/75234942/170095929-c69145a8-e5aa-46f6-84cd-efab486ab59f.png)


### Display the Eroded Image

![A2](https://user-images.githubusercontent.com/75234942/170095981-38ac44d3-0c7a-4497-b5d0-f37fc4cebe0c.png)



### Display the Dilated Image

![A3](https://user-images.githubusercontent.com/75234942/170095670-abd80834-96d9-4ac4-9a5a-cbfaf220548a.png)



## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
