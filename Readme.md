Name: Ponguru Aasrith Sairam
Reg. No: 212223240116
```
import cv2
import matplotlib.pyplot as plt

image = cv2.imread('Chichubuddi.jpg', cv2.IMREAD_GRAYSCALE)

height, width = image.shape
print(f'Width: {width}, Height: {height}')

plt.figure(figsize=[10, 10])
plt.imshow(image, cmap='gray')
plt.axis('on')  
plt.show()
cv2.imwrite('Apollo-11-launch.png', image)

import cv2
import matplotlib.pyplot as plt

image = cv2.imread('Chichubuddi.jpg')

text = 'Apollo 11 Saturn V Launch, July 16, 1969'
font_face = cv2.FONT_HERSHEY_PLAIN
font_scale = 3
font_thickness = 3
text_color = (255, 255, 255)  

text_size, _ = cv2.getTextSize(text, font_face, font_scale, font_thickness)
text_x = (image.shape[1] - text_size[0]) // 2  
text_y = image.shape[0] - 50  

cv2.putText(image, text, (text_x, text_y), font_face, font_scale, text_color, font_thickness)

magenta = (255, 0, 255)  
image_rectangle = cv2.rectangle(image, (700, 60), (500, 630), magenta, thickness=3, lineType=cv2.LINE_8)

plt.figure(figsize=[12, 12])
plt.imshow(cv2.cvtColor(image_rectangle, cv2.COLOR_BGR2RGB))
plt.axis('on')
plt.show()
```
```
import cv2
import matplotlib.pyplot as plt
image = cv2.imread('Apollo.jpg')
height=720
width=1280
print(f"Width: {width}, Height: {height}")
plt.figure(figsize=(10, 10))
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
plt.show()
cv2.imwrite('Apollo-11-Launch.png', image)
x, y, a, b = 250, 250, 250, 250
cropped_img = img[y:y+b, x:x+a]
resized_img = cv2.resize(cropped_img,None, fx=2, fy=2)
flipped_img = cv2.flip(resized_img, 1)
plt.figure(figsize=[5, 5])
plt.imshow(flipped_img[:, :, ::-1])
plt.title("Cropped, Resized, and Flipped Image")
plt.show()
img = cv2.imread('newzealand.jpg', cv2.IMREAD_COLOR)
print(img.shape)
plt.figure(figsize=[3, 3])
plt.imshow(img[:, :, ::-1])
plt.title("Original Image")
plt.show()
gray_image = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
print("Grayscale Image Shape:", gray_image.shape)
plt.figure(figsize=(10, 10))
plt.imshow(gray_image)
plt.axis('off')
plt.title("Grayscale Image")
plt.show()
```
## output
![image](https://github.com/user-attachments/assets/4ae3beda-9a80-4fb1-9296-3c78b4293ee2)
![image](https://github.com/user-attachments/assets/9dd379d1-c5d3-419e-a9d2-63964f5d11fe)
![image](https://github.com/user-attachments/assets/ca74b001-87f7-44f1-8951-3c4d775f0abe)
![image](https://github.com/user-attachments/assets/133cfeef-d451-46bd-9e5f-1425cbbba5d1)

