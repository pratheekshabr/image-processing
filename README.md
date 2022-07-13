# image-processing
<b>1.Develop a program to display gray scale image using read and write operations</b><br>
1.develop a program to display grayscal;e image in using read and write operation import cv2<br>
img=cv2.imread('leaf1.jpg',0)<br>
cv2.imshow('leaf1',img)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
output:
![image](https://user-images.githubusercontent.com/97940277/178714980-6ae7884f-eba4-4855-be33-c7dc1be01d2e.png)

<b>2.Develop a program to display the image using matplotlib</b><br>
import matplotlib.image as mpimg<br>
import matplotlib.pyplot as plt<br>
img=mpimg.imread("d1.jpg")<br>
plt.imshow(img)<br>
output:
![image](https://user-images.githubusercontent.com/97940277/178715164-f0ca5170-7d9f-4e77-a659-e9495150dca7.png)

<b>3.develop a program to perform linear transformation rotation from PIL import Image<br>
img=Image.open("plant1.jpg")<br>
img=img.rotate(180)
img.show()<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows() </b> <br>
output:
![image](https://user-images.githubusercontent.com/97940277/178715617-c3a1cac0-5bae-4fda-9a5a-66b6ed1371d3.png)

<b>4.DEVELOP PROGRAM TO CONVERT colorstring to RGB COLOR VALUES
import cv2
from PIL import ImageColor
img1=ImageColor.getrgb("yellow")
print(img1)
img1=ImageColor.getrgb("red")
print(img1)
img1=ImageColor.getrgb("pink")
print(img1)
OUTPUT:
(255, 255, 0)
(255, 0, 0)
(255, 192, 203)
5.Write a program to create image using color
from PIL import Image)
img=Image.new("RGB",(200,400),(255,255,0)))
img.show())</b>


![image](https://user-images.githubusercontent.com/97940277/178714652-4c2bc801-8aff-4be1-ae92-5c4813df62b7.png)
