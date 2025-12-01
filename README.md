# Working-on-computer-vision-OpenCv

It includes everything from reading and saving images to creating filters from scratch and video manipulation.
The goal is to understand foundational computer-vision concepts through hands-on implementation.

## 🚀 Features Implemented
## 1️⃣ Importing Libraries

Importing essential libraries such as cv2, numpy, and matplotlib.

## 2️⃣ Reading & Displaying Images

Loading images using cv2.imread()

Displaying images using cv2.imshow() and matplotlib

Converting BGR ↔ RGB

## 3️⃣ Converting Image to Black & White (Grayscale)

Using cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)

## 4️⃣ Saving Images

Saving outputs using cv2.imwrite("output.jpg", img)

## 5️⃣ Drawing on Images

Drawing lines, rectangles, circles using:

cv2.line()

cv2.rectangle()

cv2.circle()

## 6️⃣ Creating a Black Canvas

Generating black (zeros) canvas using NumPy:

canvas = np.zeros((500, 500, 3), dtype=np.uint8)

## 7️⃣ Channel Segregation & Merging

Splitting channels: b, g, r = cv2.split(img)

Merging channels: cv2.merge([b, g, r])

## 8️⃣ Image Transformations
✔ Resize

cv2.resize(img, (width, height))

✔ Crop

Using array slicing:
cropped = img[y1:y2, x1:x2]

✔ Flip

cv2.flip(img, 0) – vertical
cv2.flip(img, 1) – horizontal

✔ Rotate

Using simple rotation: cv2.rotate(img, cv2.ROTATE_90_CLOCKWISE)

Using rotation matrix for custom angles

✔ Add Images

Using cv2.add() and cv2.addWeighted()

## 9️⃣ Pixel Range Filtering

Extracting pixels using mask:

mask = cv2.inRange(img, lower_range, upper_range)

## 🔟 Thresholding

Global Threshold

Adaptive Threshold

OTSU Threshold
Using functions like:

cv2.threshold()
cv2.adaptiveThreshold()

## 1️⃣1️⃣ Filters From Scratch

Implemented custom filters using convolution:

Vertical Edge Detection Kernel

Horizontal Edge Detection Kernel

Custom blur/sharpen kernels

Using:

cv2.filter2D(img, -1, kernel)

## 1️⃣2️⃣ Video Processing

Reading video frames using cv2.VideoCapture()

Displaying each frame in real-time

Converting video frames to grayscale

## 🛠 Technologies Used

Python

OpenCV

NumPy

Matplotlib

## 🧠 What I Learned

Image fundamentals (matrix representation)

Color channel operations

Convolution & custom filtering

Transformations in computer vision

Real-time video frame manipulation

Drawing shapes on video frames

Saving processed output video
