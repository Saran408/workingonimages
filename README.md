# <p align='center'>WORKING ON IMAGES</p>

## Program:
```
# Developed By:SARAN M
# Register Number:212220230044
```

```python
import cv2
import matplotlib.pyplot as plt 
img=cv2.imread("flower.jpg",1)
img=cv2.resize(img, (400, 300))
plt.subplot(3,3,1)
plt.title('Flower (original image)') 
plt.imshow(img)

plt.rcParams["figure.figsize"] = [12, 8]

# gray image
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
plt.subplot(3,3,2)
plt.title('Gray Image') 
plt.imshow(gray)

# hsv image
hsv = cv2.cvtColor(img, cv2.COLOR_BGR2HSV)
plt.subplot(3,3,3)
plt.title("Hsv Image")
plt.imshow(hsv) 
h,s,v=cv2.split(hsv)

# h plane
plt.subplot(3,3,4)
plt.title('H plane')
plt.imshow(h)

# s plane
plt.subplot(3,3,5)
plt.title('s plane')
plt.imshow(s)

# v plane
plt.subplot(3,3,6)
plt.title('V plane')
plt.imshow(v)
```

## Output:
![image](https://user-images.githubusercontent.com/75235427/175644345-10edef71-8cdc-4699-9f71-5bfee4ea794d.png)
