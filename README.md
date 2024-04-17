# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>Import the necessary packages


### Step2:
<br>Create the Text using cv2.putText

### Step3:
<br>Create the structuring element

### Step4:
<br>Use Opening operation

### Step5:
<br>Use Closing Operation

 
## Program:
### OPENING
``` python
import numpy as np
import cv2
import matplotlib.pyplot as plt
img1=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'Batman',(5,70), font,2,(255),5,cv2.LINE_AA)
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image1=cv2.morphologyEx(img1,cv2.MORPH_OPEN,kernel)
plt.imshow(image1)
plt.axis("off")

```
### CLOSING
```python
import numpy as np
import cv2
import matplotlib.pyplot as plt
img1=np.zeros((100,400), dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'Batman',(5,70), font,2,(255),5,cv2.LINE_AA)
kernel=np.ones((5,5),np.uint8)
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image2=cv2.morphologyEx(img1,cv2.MORPH_CLOSE,kernel)
plt.imshow(image2)
plt.axis("off")
```
## Output:

### Display the input Image
<br>![Screenshot 2024-04-17 091156](https://github.com/Mathiofficial/OPENING--AND-CLOSING/assets/118787327/8b03fba2-660c-4d41-b806-b20db9a46ae3)


### Display the result of Opening
<br>![Screenshot 2024-04-17 091141](https://github.com/Mathiofficial/OPENING--AND-CLOSING/assets/118787327/5cd3059a-5990-468c-a3b7-552754893b7c)


## Display the result of Closing
<br>![Screenshot 2024-04-17 091149](https://github.com/Mathiofficial/OPENING--AND-CLOSING/assets/118787327/bc71104f-0e9c-4086-a958-05236ef84c6e)





## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
