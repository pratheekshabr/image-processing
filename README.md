# image-processing
<b>1.Develop a program to display gray scale image using read and write operations</b><br>
1.develop a program to display grayscal;e image in using read and write operation import cv2<br>
img=cv2.imread('leaf1.jpg',0)<br>
cv2.imshow('leaf1',img)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/178714980-6ae7884f-eba4-4855-be33-c7dc1be01d2e.png)

<b>2.Develop a program to display the image using matplotlib</b><br>
import matplotlib.image as mpimg<br>
import matplotlib.pyplot as plt<br>
img=mpimg.imread("d1.jpg")<br>
plt.imshow(img)<br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/178715164-f0ca5170-7d9f-4e77-a659-e9495150dca7.png)

<b>3.develop a program to perform linear transformation rotation from PIL import Image<br>
img=Image.open("plant1.jpg")<br>
img=img.rotate(180)
img.show()<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows() </b> <br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/178715617-c3a1cac0-5bae-4fda-9a5a-66b6ed1371d3.png)

<b>4.DEVELOP PROGRAM TO CONVERT colorstring to RGB COLOR VALUES
import cv2<br>
from PIL import ImageColor<br>
img1=ImageColor.getrgb("yellow")<br>
print(img1)<br>
img1=ImageColor.getrgb("red")<br>
print(img1)<br>
img1=ImageColor.getrgb("pink")<br>
print(img1)<br>
OUTPUT:<br>
(255, 255, 0)<br>
(255, 0, 0)<br>
(255, 192, 203)<br>

  <b>5.Write a program to create image using color</b><br>
from PIL import Image)<br>
img=Image.new("RGB",(200,400),(255,255,0)))<br>
img.show())</b><br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/178714652-4c2bc801-8aff-4be1-ae92-5c4813df62b7.png)<br>

<br>6.develop a program to utilize the image using various color spaces<br>
import cv2<br>
import matplotlib.pyplot as plt<br>
import numpy as np<br>
img=cv2.imread('d1.jpg')<br>
plt.imshow(img)<br>
plt.show()<br>
img=cv2.cvtColor(img,cv2.COLOR_BGR2RGB)<br>
plt.imshow(img)<br>
plt.show()<br>
img=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)<br>
plt.imshow(img)<br>
plt.show()<br>
![image](https://user-images.githubusercontent.com/97940277/178717913-670f45ec-46e7-491c-8ce2-87bc66920811.png)<br>

7.write a program to display image attributes<br>
from PIL import Image<br>
image=Image.open('d1.jpg')<br>
print("filename:",image.filename)<br>
print("mode:",image.mode)<br>
print("size:",image.size)<br>
print("width:",image.width)<br>
print("height:",image.height)
image.close()<br>
output:<br>
filename: d1.jpg<br>
mode: RGB<br>
size: (259, 194)<br>
width: 259<br>
height: 194<br>

8.Resize the original imag<br>
from PIL import Imag<br>
image=Image.open("flower2.jpg"<br>
print("Filename:",image.filename<br>
print("Format:",image.format<br>
print("Mode:",image.mode<br>
print("Size:",image.size<br>
print("Width:",image.width<br>
print("Height:",image.height<br>
image.close(<br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/178718073-94f423a6-8f30-4ae1-b811-66cca3f0a53b.png)<br>

9.convert the original to grey scale and then to binary <br>
import cv2<br>

img=cv2.imread('flower3.jpg')<br>
cv2.imshow("RGB",img)<br>
cv2.waitKey(0)<br>
#gray scale<br>
img=cv2.imread ('flower3.jpg',0)<br>
cv2.imshow("Gray",img)<br>
cv2.waitKey(0)<br>
#binary image<br>
ret,bw_img=cv2.threshold (img,127,255,cv2.THRESH_BINAR<br>
Y) cv2.imshow("Binary",bw_img)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br><br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/178718230-81e605e8-124e-40ed-ad1b-89d6c18b08aa.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178718274-b05379fa-eceb-4eaf-9317-be15bd84fe8e.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178718326-56cbe202-0e24-4937-9c92-7d3292510b01.png)<br>




Lab excercise<br>
1.cover the image to URL code<br>
from skimage import io<br><br>
import matplotlib.pyplot as plt<br>
url='https://i.natgeofe.com/n/3861de2a-04e6-45fd-aec8-02e7809f9d4e/02-cat-training-NationalGeographic_1484324_3x2.jpg'<br>
image=io.imread(url) plt.imshow(image)<br>
plt.show()<br>

output:<br>
![image](https://user-images.githubusercontent.com/97940277/178718739-bcf6c0b9-010f-4099-ba5e-2d68ad97f8d7.png)<br>


**2.Write a program to mask and blur the image **<br>
import cv2<br>
import matplotlib.image as mping<br>
import matplotlib.pyplot as plt<br>
img=cv2.imread('ow.jpg')<br>
plt.imshow(img)
plt.show()<br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/178719442-0e757f29-9c36-431e-bacf-2ed20a326e60.png)<br>


hsv_img=cv2.cvtColor(img,cv2.COLOR_RGB2HSV)<br><br>
light_orange=(1,190,200)<br><br>
dark_orange=(18,255,255)<br><br>
mask=cv2.inRange(img,light_orange,dark_orange)<br><br>
result=cv2.bitwise_and(img,img,mask=mask)<br><br><br>
plt.subplot(1,2,1)<br><br>
plt.imshow(mask,cmap="gray")<br><br>
plt.subplot(1,2,2)<br>
plt.imshow(result)<br>
![image](https://user-images.githubusercontent.com/97940277/178719520-ba663976-accd-44b9-b586-ac2a1b255b96.png)<br>


light_white=(0,0,200)<br>
dark_white=(145,60,255)<br>
mask_white=cv2.inRange(hsv_img,light_white,dark_white)<br>
result_white=cv2.bitwise_and(img,img,mask=mask_white)<br>
plt.subplot(1,2,1)<br>
plt.imshow(mask,cmap="gray")<br>
plt.subplot(1,2,2)<br>
plt.imshow(result_white)<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/97940277/178719893-0010830f-a44d-4211-a790-d41148cbfec3.png)<br>


final_mask=mask+mask_white<br>

final_result=cv2.bitwise_and(img,img,mask=final_mask)<br>
plt.subplot(1,2,1)<br>
plt.imshow(final_mask,cmap="gray")<br>
plt.subplot(1,2,2)<br><br>
plt.imshow(final_result)<br>
plt.show() image<br>
blur=cv2.GaussianBlur(final_result,(7,7),0)<br>
plt.imshow(blur)<br>
plt.show()<br>
![image](https://user-images.githubusercontent.com/97940277/178719967-f39ef39a-b4aa-426c-a437-a026e61044ae.png)<br>


3.write a program to perform arithmatic operation on images?<br>
import cv2<br>
import matplotlib.image as mping<br>
import matplotlib.pyplot as plt<br>

#reading image files<br>
img1=cv2.imread('doll1.jpg')<br>
img2=cv2.imread('doll2.jpg')<br>
<br>
#applying numpy additional on images<br>
fimg1=img1+img2<br>
plt.imshow(fimg1)<br>
plt.show()<br>

#Saving the output image<br>
cv2.imwrite('output.jpg',fimg1)<br>
fimg2=img1-img2<br>
plt.imshow(fimg2)<br>
plt.show()<br>

#saving the output image<br>
cv2.imwrite('output.jpg',fimg2)<br>
fimg3=img1*img2<br>
plt.imshow(fimg3)<br>
plt.show()<br><br>

#saving the output image<br>
cv2.imwrite('output.jpg',fimg3)<br>
fimg4=img1/img2<br>
plt.imshow(fimg4)<br>
plt.show()<br>

#saving the output image<br>
cv2.imwrite('output.jpg',fimg4)<br>

![image](https://user-images.githubusercontent.com/97940277/178959748-3e3bd558-a612-4234-a9f1-b6c709986966.png)<br>

![image](https://user-images.githubusercontent.com/97940277/178959801-e20b90ea-d197-4c46-8188-17504200b67e.png)<br>

![image](https://user-images.githubusercontent.com/97940277/178959841-f60a3bc6-b162-477e-a117-280479858fee.png)<br>



4.write a program to image to different color space
import cv2
img=cv2.imread("D:\red.jpg")<br>
gray=cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)<br>
hsv=cv2.cvtColor(img,cv2.COLOR_BGR2HSV)<br>
lab=cv2.cvtColor(img,cv2.COLOR_BGR2LAB)<br>
hls=cv2.cvtColor(img,cv2.COLOR_BGR2HLS)<br>
yuv=cv2.cvtColor(img,cv2.COLOR_BGR2YUV)<br>
cv2.imshow("GRAY image",gray)<br>
cv2.imshow("HSV image",hsv)<br>
cv2.imshow("LAB image",lab)<br><br>
cv2.imshow("HLS image",hls)<br>
cv2.imshow("YUV image",yuv)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/178959979-7b7bee01-ca37-424e-bdb9-9146a9b27dcb.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178961160-12aa4ad0-c6b3-4d5d-888c-5ae9f1175754.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178961197-c8b9e5d2-74f8-4825-905d-94c418c8363d.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178961237-c232087d-ae43-4dde-bbf7-347254023580.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178961292-952e8568-cb52-4e98-9209-c8dc787eb673.png)<br>


5.program to create an image using 2Darray<br>

import cv2 as c<br>
import numpy as np<br>
from PIL import Image<br>
array=np.zeros([255,130,3],dtype=np.uint8)<br>
array[:,:100]=[255,130,0]<br>
array[:,100:]=[0,0,255]<br>
img=Image.fromarray(array)<br>
img.save('image1.png')<br>
img.show()<br><br>
c.waitKey(0)<br>

![image](https://user-images.githubusercontent.com/97940277/178961601-9ff2d0c5-c1ed-4cd2-a732-5a7dd4a8d334.png)<br>

6.Image processing using bitwise operator?<br><br>

import cv2<br><br>
import matplotlib.pyplot as plt<br>
image1=cv2.imread('nature.jpg')<br><br>
image2=cv2.imread('nature.jpg')<br>
ax=plt.subplots(figsize=(15,10))<br>
bitwiseAnd=cv2.bitwise_and (image1,image2)<br>
bitwiseOr=cv2.bitwise_or (image1,image2)<br>
bitwiseXor=cv2.bitwise_xor (image1,image2)<br>
bitwiseNot_img1=cv2.bitwise_not (image1,image2)<br>
bitwiseNot_img2=cv2.bitwise_not (image1,image2)<br>
plt.subplot(151)<br>
plt.imshow(bitwiseAnd)<br>
plt.subplot(152)<br>
plt.imshow(bitwiseOr)<br>
plt.subplot(153)<br><br>
plt.imshow(bitwiseXor)<br>
plt.subplot(154)<br>
plt.imshow(bitwiseNot_img1)<br>
plt.subplot(155)<br>
plt.imshow(bitwiseNot_img2)<br>
cv2.waitKey(0)<br>

Output:<br>
![image](https://user-images.githubusercontent.com/97940277/178962555-312d6f92-7ac9-4bde-beea-12a1d6273a26.png)<br>

7.blur image<br>
import cv2<br>
import numpy as np<br><br>

image=cv2.imread('puppy2.jpg')<br>

cv2.imshow('original Image',image)<br>
cv2.waitKey(0)<br>

#gaussian blur<br>
Gaussian=cv2.GaussianBlur(image,(7,7),0)<br>
cv2.imshow('Gaussian Blurring',Gaussian)<br>
cv2.waitKey(0)<br>

#median Blur<br>
median=cv2.medianBlur(image,5)<br>
cv2.imshow('Median Blurring',median)<br>
cv2.waitKey(0)<br>

#Bilateral Blur<br>
bilateral=cv2.bilateralFilter(image,9,75,75)<br>
cv2.imshow('Bilateral Blurring',bilateral)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
<br>
ouput:<br>
image image image image<br>

8.Image enhancement from PIL import Image from PIL import ImageEnhance image=Image.open('nature.jpg') image.show()<br>

enh_bri=ImageEnhance.Brightness(image) brightness=1.5 image_brightned=enh_bri.enhance(brightness) image_brightned.show()<br>

enh_col=ImageEnhance.Color(image) color=1.5 image_colored=enh_col.enhance(color) image_colored.show()<br>

enh_con=ImageEnhance.Contrast(image) contrast=1.5 image_contrasted=enh_col.enhance(contrast) image_contrasted.show()<br>

enh_sha=ImageEnhance.Sharpness(image) sharpness=3.0 image_sharped=enh_sha.enhance(sharpness) image_sharped.show()
<br>
Output:<br>
image image image image image<br>

9.morphological import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
from PIL import Image,ImageEnhance<br><br>
img=cv2.imread('nature.jpg',0)<br>
ax=plt.subplots(figsize=(20,10))<br>
kernel=np.ones((5,5),np.uint8)<br>
opening=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)<br>
closing=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)<br>
erosion=cv2.erode(img,kernel,iterations=1)<br>
dilation=cv2.dilate(img,kernel,iterations=1)<br>
gradient=cv2.morphologyEx(img,cv2.MORPH_GRADIENT,kernel)<br>
plt.subplot(151)<br>
plt.imshow(opening)<br>
plt.subplot(152)<br>
plt.imshow(closing)<br>
plt.subplot(153)<br>
plt.imshow(erosion)<br>
plt.subplot(154)<br><br>
plt.imshow(dilation)<br>
plt.subplot(155)
plt.imshow(gradient)
cv2.waitKey(0)

image

10.Develop a program to

i)Read the image convert it nto grayscale image<br><br>
ii)Write (save) the grayscale image and<br>
iii)display the original image and gray scale image<br>
import cv2<br>
OriginalImg=cv2.imread('rabbit.jpg')<br>
GrayImg=cv2.imread('rabbit.jpg',0)<br>
isSaved=cv2.imwrite('D:/i.jpg',GrayImg) cv2.imshow('Display original Image',OriginalImg)<br>
cv2.imshow('Display Grayscale image',GrayImg)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
if saved:<br>
print('the image is sucessfully saved')<br>
output:<br>
image
image<br>

11.graylevel slicing with background<br>
import cv2<br><br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
image=cv2.imread('cat.jpg',0)<br>
x,y=image.shape<br>
z=np.zeros((x,y))<br>
for i in range(0,x):<br>
for j in range(0,y):<br>
if(image[i][j]>50 and image[i][j]<150):<br>
z[i][j]=255<br>
else:<br>
z[i][j]=image[i][j]<br>
equ=np.hstack((image,z))<br>
plt.title('graylevel slicing with background')<br>
plt.imshow(equ,'gray')<br>
plt.show()<br>
image<br>

12.graylevel slicing without background<br>
import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
image=cv2.imread('cat.jpg',0)<br>
x,y=image.shape<br>
z=np.zeros((x,y))<br>
for i in range(0,x):<br>
for j in range(0,y):<br>
if(image[i][j]>50 and image[i][j]<150):<br>
z[i][j]=255<br>
else:<br>
z[i][j]=0<br>
equ=np.hstack((image,z))<br>
plt.title('graylevel slicing without background')<br>
plt.imshow(equ,'gray')<br>
plt.show()<br>
image
<br>

