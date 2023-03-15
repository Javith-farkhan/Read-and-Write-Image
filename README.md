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
  pic=cv2.imread("Dip_image.jfif",1)
  cv2.imshow("212221240017",pic)
  cv2.waitKey(0)
  cv2.destroyAllWindows() 

```
ii) #To write the image
```
import cv2
pic=cv2.imread("Dip_image.jfif",1)
cv2.imshow("212221240017",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
iii) #Find the shape of the Image
```
import cv2
pic = cv2.imread('Dip_image.jfif',1)
print(pic.shape)

```
iv) #To access rows and columns

```
import cv2
import random
pic=cv2.imread("Dip_image.jfif",1)
for i in range(100):
    for j in range(pic.shape[1]):
        pic[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("212221240017",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
v) #To cut and paste portion of image
```
import cv2
pic=cv2.imread("Dip_image.jfif",1)
crop=pic[150:180,150:180]
pic[82:100,70:100]=crop
cv2.imshow("212221240017",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

## Output:

### i) Read and display the image

![Dip 1 1](https://user-images.githubusercontent.com/94296805/225331435-098398ce-e4c3-43e0-8d6b-ea497a1eefcf.png)



### ii)Write the image

![Dip 1 2](https://user-images.githubusercontent.com/94296805/225331642-057df543-a179-4d84-87e2-54752193948e.png)


### iii)Shape of the Image

![Dip 1 3](https://user-images.githubusercontent.com/94296805/225331813-dc1d586e-d9e0-4de6-bec0-86eed372a389.png)



### iv)Access rows and columns

![Dip 1 4](https://user-images.githubusercontent.com/94296805/225331900-aa35c814-0026-4cbe-beed-b63a08527bd2.png)


### v)Cut and paste portion of image

![Dip 1 5](https://user-images.githubusercontent.com/94296805/225331954-76df806a-2070-470e-9140-c15cab1b7df5.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


