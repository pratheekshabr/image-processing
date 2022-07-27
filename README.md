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

<b>3.develop a program to perform linear transformation rotation from PIL import Image</b><br>
img=Image.open("plant1.jpg")<br>
img=img.rotate(180)
img.show()<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows() </b> <br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/178715617-c3a1cac0-5bae-4fda-9a5a-66b6ed1371d3.png)

<b>4.Develop Program to convert colorstring to RGB Color values</b><br>
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

<b><br>6.develop a program to utilize the image using various color spaces</b><br>
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

<b>7.write a program to display image attributes</b><br>
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

<b>8.Resize the original image</b><br>
import cv2<br>
img=cv2.imread('flower1.jpg')<br>
print('original image length width',img.shape)<br>
cv2.imshow('original image',img)<br>
cv2.waitKey(0)<br>
#to show the resized image<br>
imgresize=cv2.resize(img,(150,160))<br>
cv2.imshow('Resized image',imgresize)<br>
print('resized image lenght width',imgresize.shape)<br>
cv2.waitKey(0)<br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/178969992-f5f49c45-8628-40a9-afba-37611a58b6b7.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178970033-b932113c-695c-4878-ad97-3e1515692309.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178970358-c68f01ef-7e19-48f0-938d-9eb3f7142497.png)<br>


<b>9.convert the original to grey scale and then to binary</b> <br>
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
<b>1.cover the image to URL code</b><br>
from skimage import io<br><br>
import matplotlib.pyplot as plt<br>
url='https://i.natgeofe.com/n/3861de2a-04e6-45fd-aec8-02e7809f9d4e/02-cat-training-NationalGeographic_1484324_3x2.jpg'<br>
image=io.imread(url) plt.imshow(image)<br>
plt.show()<br>

output:<br>
![image](https://user-images.githubusercontent.com/97940277/178718739-bcf6c0b9-010f-4099-ba5e-2d68ad97f8d7.png)<br>


<b>2.Write a program to mask and blur the image </b><br>
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


<b>3.write a program to perform arithmatic operation on images</b><br>
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



<b>4.write a program to image to different color space</b><br>
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


<b>5.program to create an image using 2Darray</b><br>

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

<b>6.Image processing using bitwise operator?</b><br>

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

<b>7.blur image</b><br>
import cv2<br>
import numpy as np<br><br>

image=cv2.imread('img1.jpg')<br>

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
![image](https://user-images.githubusercontent.com/97940277/178963497-95b95e6f-bdac-4dd4-963a-3821f2e6e1f2.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178963597-fb3f4b1e-fffb-4c56-91f8-8cef9d30bcd5.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178963707-2aab2b8e-716e-400f-a4c1-b3ce03378f51.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178963808-69aff8c8-c3e7-4a8c-b9d2-8b99a26083f9.png)<br>



<b>8.Image enhancement</b><br>
from PIL import Image <br>
from PIL import ImageEnhance <br>
image=Image.open('nature.jpg') <br>
image.show()<br>
enh_bri=ImageEnhance.Brightness(image)<br>
brightness=1.5 <br>
image_brightned=enh_bri.enhance(brightness) <br>
image_brightned.show()<br>
enh_col=ImageEnhance.Color(image) <br>
color=1.5 <br>
image_colored=enh_col.enhance(color)<br>
image_colored.show()<br>
enh_con=ImageEnhance.Contrast(image)<br>
contrast=1.5<br>
image_contrasted=enh_col.enhance(contrast) <br>
image_contrasted.show()<br><br>
enh_sha=ImageEnhance.Sharpness(image) <br>
sharpness=3.0 <br>
image_sharped=enh_sha.enhance(sharpness) <br>
image_sharped.show()<br>

Output:<br>
![image](https://user-images.githubusercontent.com/97940277/178964842-98026394-6cc7-4df8-8def-544709ecb2c1.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178964989-e2188b15-8d0f-465e-896e-4211443e38c4.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178965136-b4e0b66e-7f43-4940-936d-fe1a86c9d2ab.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178965388-049b7efa-f03d-4cc9-b0d8-28873b4cc93e.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178965455-0e1fa11d-af59-4fdf-9490-5aae9da7e325.png)<br>



<b>9.morphological </b><br>
import cv2<br>
import numpy as np<br>
from matplotlib import pyplot as plt<br>
from PIL import Image,ImageEnhance<br><br>
img=cv2.imread('tj.jpg',0)<br>
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
plt.subplot(155)<br>
plt.imshow(gradient)<br>
cv2.waitKey(0)<br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/178966916-1772b3bd-5108-42d9-85fe-58dc632188a0.png)<br>




<b>10.Develop a program to
i)Read the image convert it nto grayscale image<br>
ii)Write (save) the grayscale image and<br>
iii)display the original image and gray scale image<br>
import cv2</b><br>
OriginalImg=cv2.imread('rabbit.jpg')<br>
GrayImg=cv2.imread('rabbit.jpg',0)<br>
isSaved=cv2.imwrite('D:/i.jpg',GrayImg) <br>
cv2.imshow('Display original Image',OriginalImg)<br>
cv2.imshow('Display Grayscale image',GrayImg)<br>
cv2.waitKey(0)<br>
cv2.destroyAllWindows()<br>
if saved:<br>
print('the image is sucessfully saved')<br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/178967628-d19f0ee9-c6cc-4e40-a89b-44eafef2b393.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178967711-f1a39883-2a42-4613-9182-feb487bd373c.png)<br>

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
![image](https://user-images.githubusercontent.com/97940277/178971021-11356c05-51f6-4643-8018-83e266ab49fd.png)<br>

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
![image](https://user-images.githubusercontent.com/97940277/178971069-841184c4-6139-42e3-b45a-7aec654a47b8.png)<br>


13. import numpy<br>
import numpy as np<br>
img  = cv2.imread('puppy.jpg',0)<br>
hist = cv2.calcHist([img],[0],None,[256],[0,256])<br>
plt.hist(img.ravel(),256,[0,256])<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/97940277/178972022-a049dc4d-d317-4ef4-9ff5-23ebd96ed19f.png)<br>
  
  #skiimg <br>
from skimage import io<br>
import matplotlib.pyplot as plt<br>
image = io.imread('puppy.jpg')<br>
_ = plt.hist(image.ravel(), bins = 256, color = 'orange', )<br>
_ = plt.hist(image[:, :, 0].ravel(), bins = 256, color = 'red', alpha = 0.5)<br>
_ = plt.hist(image[:, :, 1].ravel(), bins = 256, color = 'Green', alpha = 0.5)
_ = plt.hist(image[:, :, 2].ravel(), bins = 256, color = 'Blue', alpha = 0.5)<br>
_ = plt.xlabel('Intensity Value')<br>
_ = plt.ylabel('Count')<br>
_ = plt.legend(['Total', 'Red_Channel', 'Green_Channel', 'Blue_Channel'])<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/97940277/178972127-d414ae9e-266e-42a8-a179-c7b0c2e6f3ec.png)<br>

#matplot<br>
import cv2  <br><br>
from matplotlib import pyplot as plt  <br>
img = cv2.imread('img1.jpg',0) <br>
histr = cv2.calcHist([img],[0],None,[256],[0,256]) <br>
plt.plot(histr) <br>
plt.show()<br>
![image](https://user-images.githubusercontent.com/97940277/178972230-8504461a-c763-4309-a5c8-2b2ffc972473.png)<br>

import numpy as np<br>
import cv2 as cv<br>
from matplotlib import pyplot as plt<br>
img = cv.imread('img1.jpg')<br>
plt.imshow(img)<br><br>
plt.show()<br>
img = cv.imread('img1.jpg',0)<br>
plt.hist(img.ravel(),256,[0,256]);<br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/97940277/178972305-f2e0d53a-dd7c-40f2-af6c-93b53ee53058.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178972354-29cf073c-97b6-4475-8ed1-0045fec07d1e.png)<br>


from skimage import io<br>
import matplotlib.pyplot as plt<br>
img = io.imread('puppy.jpg')<br>
plt.imshow(img)<br>
plt.show()<br>
image = io.imread('puppy.jpg')<br>
ax = plt.hist(image.ravel(), bins = 256)<br><br>
plt.show()<br>

![image](https://user-images.githubusercontent.com/97940277/178972402-8910f18f-383e-4392-be67-49e81f598bb1.png)<br>
![image](https://user-images.githubusercontent.com/97940277/178972455-2ca9ad8c-c55f-45ce-8516-6beeff5e8079.png)<br>


<b>1. Program to perform basic image data analysis using intensity transformation:<br>
a) Image negative<br>
b) Log transformation<br>
c) Gamma correction</b><br>
<br>
%matplotlib inline<br>
import imageio<br>
import matplotlib.pyplot as plt<br>
import warnings<br>
import matplotlib.cbook<br>
warnings.filterwarnings("ignore",category=matplotlib.cbook.mplDeprecation)<br>
pic=imageio.imread('bunny.jpg')<br>
plt.figure(figsize=(6,6))<br>
plt.imshow(pic);<br>
plt.axis('off');<br><br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/179957210-112531e2-756b-4107-b63e-8387318457df.png)<br>


negative=255-pic #neg =(L-1) - img<br>
plt.figure(figsize=(6,6))<br>
plt.imshow(negative);<br>
plt.axis('off');<br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/179957372-c634c061-dd9d-49be-92bf-a16f44eddfb1.png)<br>


%matplotlib inline<br>

import imageio<br><br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>

pic=imageio.imread('bunny.jpg')<br>
gray=lambda rgb : np.dot(rgb[...,:3],[0.299,0.587,0.114])<br>
gray=gray(pic)<br>

max_=np.max(gray)<br>

def log_transform():<br>
    return(255/np.log(1+max_))*np.log(1+gray)<br>
plt.figure(figsize=(5,5))<br>
plt.imshow(log_transform(),cmap=plt.get_cmap(name='gray'))<br><br>
plt.axis('off');<br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/179957511-21d86811-5c8b-4e90-85e8-4c1a85d78ad0.png)<br>


import imageio<br>
import matplotlib.pyplot as plt<br>

#Gamma encoding<br>
pic=imageio.imread('bunny.jpg')<br>
gamma=2.2#Gamma <1 ~ Dark ; Gamma >1 ~ Bright<br>

gamma_correction=((pic/255)**(1/gamma))<br>
plt.figure(figsize=(5,5))<br>
plt.imshow(gamma_correction)<br>
plt.axis('off');<br>
output:<br>
![image](https://user-images.githubusercontent.com/97940277/179957646-5c867267-cb46-4f22-8ed6-6ee02f2958ae.png)<br>


<b>Program to perform basic image manipulation:<br>
a) Sharpness<br>
b) Flipping<br>
c) Cropping</b><br>
<br>
#image sharpen<br>
from PIL import Image<br>
from PIL import ImageFilter<br>
import matplotlib.pyplot as plt<br><br>
#Load the image<br>
my_image=Image.open('donkey.jpg')<br>
#Use sharpen function<br>
sharp=my_image.filter(ImageFilter.SHARPEN)<br>
#Save the image<br>
sharp.save('D:/image_sharpen.jpg')<br>
sharp.show()<br>
plt.imshow(sharp)<br>
plt.show()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/97940277/179964006-282fb479-951a-43a5-911d-0037b147af78.png)<br>

#Image flip<br>
import matplotlib.pyplot as plt<br>
#Load the image<br>
img=Image.open('donkey.jpg')<br>
plt.imshow(img)<br><br>
plt.show()<br>
#use the flip function<br>
flip=img.transpose(Image.FLIP_LEFT_RIGHT)<br>
#save the image<br>
flip.save('D:/image_flip.jpg')<br>
plt.imshow(flip)<br>
plt.show()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/97940277/179964392-6f4ecde3-660f-4574-9186-79c322a96a90.png)<br>

#Importing image class from PIL module<br>
from PIL import Image<br>
import matplotlib.pyplot as plt<br>
#Opens a image in RGB mode<br>
im=Image.open('donkey.jpg')<br>

#Size of the image in pixels(size of original image)<br>
#(This is not mandatory)<br>
width,height=im.size<br>

#Cropped image of above dimension<br>
#(It will not change the original image)<br>
im1=im.crop((280,100,800,600))<br>
#Shiws the image in image viewer<br>
im1.show()<br>
plt.imshow(im1)<br>
plt.show()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/97940277/179964521-1f5e332d-b847-4272-b5a0-de70b19d7b12.png)<br>

<b>Converting matrix to image</br>
from PIL import Image<br>
import numpy as np<br>

w, h = 512, 512<br>
data = np.zeros((h, w, 3), dtype=np.uint8)<br>
data[0:256, 0:256] = [0, 255, 0] # red patch in upper left<br>
img = Image.fromarray(data, 'RGB')<br>
img.save('my.png')<br>
img.show()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/97940277/180192388-f2782654-a047-4e27-a698-aba6d962f4d8.png)<br>

<b>Grayscale gradient<b><br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>

x = np.linspace(10,6, 100)<br>
image = np.tile(x, (100, 1)).T<br>

plt.imshow(image, cmap='gray')<br>
plt.show()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/97940277/180196125-52e75dcd-f947-453e-b465-cec2ed3a3208.png)<br>
<br>

<b>Fill circle with grayscale gradient</b><br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>

arr = np.zeros((256,256,3), dtype=np.uint8)<br>
imgsize = arr.shape[:2]<br>
innerColor = (255, 255, 255)<br>
outerColor = (0, 0, 0)<br>
for y in range(imgsize[1]):<br>
    for x in range(imgsize[0]):<br>
        #Find the distance to the center<br>
        distanceToCenter = np.sqrt((x - imgsize[0]//2) ** 2 + (y - imgsize[1]//2) ** 2)<br>

        #Make it on a scale from 0 to 1innerColor<br>
        distanceToCenter = distanceToCenter / (np.sqrt(2) * imgsize[0]/2)<br>

        #Calculate r, g, and b values<br>
        r = outerColor[0] * distanceToCenter + innerColor[0] * (1 - distanceToCenter)<br>
        g = outerColor[1] * distanceToCenter + innerColor[1] * (1 - distanceToCenter)<br>
        b = outerColor[2] * distanceToCenter + innerColor[2] * (1 - distanceToCenter)<br>
        # print r, g, b<br>
        arr[y, x] = (int(r), int(g), int(b))<br>
plt.imshow(arr, cmap='gray')<br>
plt.show()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/97940277/180193871-4cbf9f2c-e580-485f-8b75-e7d4f60b6245.png)<br>

<b>Fill circle with color gradient</b><br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
<br>
arr = np.zeros((256,256,3), dtype=np.uint8)<br>
imgsize = arr.shape[:2]<br>
innerColor = (255, 255, 255)<br>
outerColor = (0, 100, 100)<br>
for y in range(imgsize[1]):<br>
    for x in range(imgsize[0]):<br>
        #Find the distance to the center<br>
        distanceToCenter = np.sqrt((x - imgsize[0]//2) ** 2 + (y - imgsize[1]//2) ** 2)<br>

        #Make it on a scale from 0 to 1innerColor<br>
        distanceToCenter = distanceToCenter / (np.sqrt(2) * imgsize[0]/2)<br>

        #Calculate r, g, and b values<br>
        r = outerColor[0] * distanceToCenter + innerColor[0] * (1 - distanceToCenter)<br>
        g = outerColor[1] * distanceToCenter + innerColor[1] * (1 - distanceToCenter)<br>
        b = outerColor[2] * distanceToCenter + innerColor[2] * (1 - distanceToCenter)<br>
        # print r, g, b<br>
        arr[y, x] = (int(r), int(g), int(b))<br>

plt.imshow(arr, cmap='gray')<br>
plt.show()<br>
Output:<br>
![image](https://user-images.githubusercontent.com/97940277/180194316-3afb44a0-128c-4a2f-8550-4473003e71a9.png)<br>

 <b>gradient</b><br>
 from PIL import Image<br>
import matplotlib.pyplot as plt<br>
  
# Create an image as input:<br>
input_image = Image.new(mode="RGB", size=(400, 400),color="blue")<br>
  
                        
# save the image as "input.png"<br>
#(not mandatory)<br>
#input_image.save("input", format="png")<br>
  
# Extracting pixel map:<br>
pixel_map = input_image.load()<br>
  
# Extracting the width and height<br>
# of the image:<br>
width, height = input_image.size<br>
z = 100<br>
for i in range(width):<br>
    for j in range(height):<br>
        
        # the following if part will create<br>
        # a square with color orange<br>
        if((i >= z and i <= width-z) and (j >= z and j <= height-z)):<br>
            
            # RGB value of orange.<br>
            pixel_map[i, j] = (255, 165, 255)<br>

        # the following else part will fill the<br>
        # rest part with color light salmon.<br>
        else:<br>
            
            # RGB value of light salmon.<br>
            pixel_map[i, j] = (255, 160, 0)<br>
  
# The following loop will create a cross<br>
# of color blue.<br>
for i in range(width):<br>
    
    # RGB value of Blue.<br>
    pixel_map[i, i] = (0, 0, 255)<br>
    pixel_map[i, width-i-1] = (0, 0, 255)<br>
  
# Saving the final output<br>
# as "output.png":<br>
#input_image.save("output", format="png")<br>
plt.imshow(input_image)<br>
plt.show()  <br>
# use input_image.show() to see the image on the<br>
# output screen.<br>
Output:<br>
![image](https://user-images.githubusercontent.com/97940277/180200737-78131d59-eb23-4471-8634-0fe50a9ec9c7.png)<br>
                                                                    
  from PIL import Image<br>
import numpy as np<br>
w, h = 512, 512<br>
data = np.zeros((h, w, 3), dtype=np.uint8)<br>
data[0:100, 0:100] = [255, 0, 0]<br>
data[100:200, 100:200] = [255, 0, 255]<br>
data[200:300, 200:300] = [0, 255, 0]<br>
# red patch in upper left<br>
img = Image.fromarray(data, 'RGB')<br>
img.save('my.png')<br>
plt.imshow(img)<br>
plt.show()   <br>                                                               
Output:<br>
 ![image](https://user-images.githubusercontent.com/97940277/180202933-58200f0f-68bc-4269-92da-8d6033214275.png)<br>

<h1>ASSIGNMENT WORK</h1><br>
Finding the average of an image<br>
#average<br>
import imageio<br>
import matplotlib.pyplot as plt<br>
img=imageio.imread("cougar.jpg")<br>
plt.imshow(img)<br>
np.average(img)<br>
Output:<br>
![image](https://user-images.githubusercontent.com/97940277/181231102-80b31acd-42fa-4c57-81b4-5406b754e2f9.png)<br>

#standard deviation<br>
from PIL import Image,ImageStat<br>
import matplotlib.pyplot as plt<br>
im=Image.open('cougar.jpg')<br>
plt.imshow(im)<br>
plt.show()<br><br>
stat=ImageStat.Stat(im)<br>
print(stat.stddev)<br>
Output:<br>
![image](https://user-images.githubusercontent.com/97940277/181231384-2cf60bfe-82d5-4bb5-8ac2-379df02ff989.png)<br>

#Max<br>
import imageio<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
img=imageio.imread('black.jpg' )<br>
plt.imshow(img)<br>
plt.show()<br>
max_channels = np.amax([np.amax(img[:,:,0]), np.amax(img[:,:,1]),np.amax(img[:,:,2])])<br>

print(max_channels)<br>
Output:<br>
![image](https://user-images.githubusercontent.com/97940277/181231610-80cbb6d1-f856-4125-8382-2cd9f4a8f889.png)<br>

#Min<br>
import imageio<br>
import numpy as np<br>
import matplotlib.pyplot as plt<br>
img=imageio.imread('zebra.jpg' )<br>
plt.imshow(img)<br>
plt.show()<br>
min_channels = np.amin([np.min(img[:,:,0]), np.amin(img[:,:,1]),np.amin(img[:,:,2])])<br>

print(min_channels)<br>
Output:<br>
![image](https://user-images.githubusercontent.com/97940277/181231801-16327a15-de96-4477-b8ab-e4bc487d7311.png)<br>
<h1>



                                                                    
                                                                    
                                                                    

