# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By:HANUMANTH
### Register Number: 212222240016
i) #To Read,display the image
```python
  ### Developed By: HANUMANTH
### Register Number: 212222240016
import cv2
spd_mn=cv2.imread('flower.jpg',1)
cv2.imshow('HANUMANTH(22005234)',spd_mn)
cv2.waitKey(0)
  


```
ii) #To write the image
```python
### Developed By: Hanumanth
### Register Number: 212222240016

import cv2
A=cv2.imread("flower.jpg",1)
cv2.imwrite("flower.jpg",A)
cv2.imshow("HANUMANTH(22005234)",A)
cv2.waitKey(0)







```
iii) #Find the shape of the Image
```python

### Developed by : HANUMANTH
### Reference no:21222240016

import cv2 
colorImage = cv2.imread('flower.jpg',1)
print(colorImage.shape)





```
iv) #To access rows and columns

```python

### Developed by : HANUMANTH
### Reference no:21222240016
import random
import cv2
A=cv2.imread("flower.jpg",1)
for i in range(100):
    for j in range(A.shape[1]):
        A[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("HANUMANTH(212222240067)",A)
cv2.waitKey(0)




```
v) #To cut and paste portion of image
```python

### Developed by:HANUMANTH
### Reference no: 21222240016

import cv2
color_img = cv2.imread('flower.jpg',1)
tag = color_img[20:80,20:80]
color_img[90:150,90:150] = tag
cv2.imshow('Cut And Paste',color_img)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image

![OUTPUT](/1.png)

### ii)Write the image
![OUTPUT](/2.png)

<br>
<br>

### iii)Shape of the Image
![OUTPUT](/3.png)

<br>
<br>

### iv)Access rows and columns
![OUTPUT](/4.png)

<br>
<br>

### v)Cut and paste portion of image
![OUTPUT](/5.png)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


