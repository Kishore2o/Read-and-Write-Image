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
color_img=cv2.imread('212222240050(Kishore).jpg',1)
cv2.imshow('212222240050(Kishore)',color_img)
cv2.waitKey(0)

```
ii) #To write the image
```
import cv2
color_img=cv2.imread('212222240050(Kishore).jpg',1)
w=cv2.imwrite('1.jpg',color_img)
cv2.imshow('212222240050(Kishore)',color_img)
cv2.waitKey(0)


```
iii) #Find the shape of the Image
```
import cv2
colorImage = cv2.imread('212222240050(Kishore).jpg',1)
print(colorImage.shape)



```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('212222240050(Kishore).jpg',1)
for i in range(100):
for j in range(color_img.shape[1]):
color_img[i][j]=[random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222240050(Kishore)',color_img)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```
import cv2
color_img = cv2.imread('212222240050(Kishore).jpg',1)
tag = color_img[20:80,20:80]
color_img[90:150,90:150] = tag
cv2.imshow('212222240050(Kishore)',color_img)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image
![image](https://user-images.githubusercontent.com/118679883/224110138-e9c0acd8-adaf-4534-aa98-8832848f93cb.png)



### ii)Write the image
file:///home/sec/Pictures/Screenshots/212222240050(Kishore).jpg![image](https://user-images.githubusercontent.com/118679883/224110272-2d9a4856-3367-4140-9ef3-666f8fc1d5b8.png)



### iii)Shape of the Image
file:///home/sec/Pictures/Screenshots/Screenshot%20from%202023-03-09%2023-09-47.png![image](https://user-images.githubusercontent.com/118679883/224110432-49408a43-f825-42a8-bf43-666b56fe122b.png)


### iv)Access rows and columns


### v)Cut and paste portion of image


## Result:
Thus the images are read, displayed, and written successfully using the python program.


