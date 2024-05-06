# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages


### Step2:
Create the Text using cv2.putText

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

 
## Program:
```
Developed by: SAKTHIVEL R
Register Number: 212222100044
```

# Display the input Image
```
import cv2
import numpy as np

img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'SPIDY', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)
```


# Create ths structured element
```
struct_ele = np.ones((9, 9), np.uint8)
```


# Display the result of Opening
```
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)
```
# Display the result of Closing
```
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)
```
## Output:

### Display the input Image

![Screenshot 2024-04-28 103128](https://github.com/Gokul0117/OPENING--AND-CLOSING/assets/121165938/1ff75347-8619-4c7a-9623-8ae21ab20af2)


### Display the result of Opening

![Screenshot 2024-04-28 103215](https://github.com/Gokul0117/OPENING--AND-CLOSING/assets/121165938/c6ecea4d-0652-4e42-a00f-c8b00b74e98c)


### Display the result of Closing

![Screenshot 2024-04-28 103242](https://github.com/Gokul0117/OPENING--AND-CLOSING/assets/121165938/977902e4-43f6-499e-a2bd-fa458b3c46cc)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
