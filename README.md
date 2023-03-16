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
### Developed By:
### Register Number: 
i) #To Read,display the image
```
import cv2
color= cv2.imread('rose.jpg',1)
cv2.imshow('nivetha212221240034',color)
cv2.waitKey(0)
  

```
ii) #To write the image
```
import cv2
color= cv2.imread('rose.jpg',-1)
cv2.imwrite('rose.jpg',color)


```
iii) #Find the shape of the Image
```python3
import cv2
color=cv2.imread('rose.jpg',1)
print(color.shape)


```
iv) #To access rows and columns

```python3

import cv2
import random
img= cv2.imread('rose.jpg',-1)
for i in range(300):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('nivetha212221240034',img)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```python3

import cv2
img1=cv2.imread('rose.JPG',-1)
copied_portion=img1[10:60,10:120]
img1[110:160,110:220]=copied_portion
cv2.imshow('nivetha212221240034',img1)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

## Output:

### i) Read and display the image

![output](./img1.png)

### ii)Write the image
![output](./img2.png)


### iii)Shape of the Image
![output](./img3.png)


### iv)Access rows and columns
![output](./img4.png)

### v)Cut and paste portion of image
![output](./img5.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


