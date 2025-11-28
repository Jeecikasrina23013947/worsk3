# worsk3
## Reg No: 212223100015
## Name: JEECIKASRINA M
# AIM :
To perform edge detection on an image using the Canny edge detection algorithm after applying Gaussian smoothing to reduce noise.
# PROGRAM :
```
import cv2
import matplotlib.pyplot as plt
# Read the image
img = cv2.imread('img1.jpeg',cv2.IMREAD_GRAYSCALE)
# Apply Gaussian blur to reduce noise
blurred =cv2.GaussianBlur(img, (5,5),0)
# Detect edges using Canny
edges = cv2.Canny(blurred, 50, 150) #Adjust threshold values as needed
# Plot the original image and the detected edges
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()
```
# OUTPUT :
<img width="866" height="532" alt="image" src="https://github.com/user-attachments/assets/08fd52e6-eca6-4645-82a4-355a5bf7b30b" />

# RESULT :
The output clearly shows the prominent boundaries and structural details of the image.
