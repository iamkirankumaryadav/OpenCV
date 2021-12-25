### `Open Computer Vision`

```python
!pip install opencv-contrib-python
import cv2
```
- An open source computer vision and machine learning `library`.
- Contains over 2,500 optimized algorithms.
- Algorithms for Facial recognition, Object identification, Human action, Track movements,etc.
- Computers gain high level understanding from digital `image` and `video`
- Understand and automate the task of `human visual system`
- `Detecting` and `labelling` image or object has surpassed humans.
- `Faster` than human reaction and `99% Accuracy`
- High amount of visual data i.e images and videos with high processing capabilities.

```
OpenCV and NumPy
```
- `OpenCV` code is orignally written in `C++`
- When we use OpenCV in Python, Python act as `wrapper` around C++ Code. 
- All the `OpenCV array` structures are converted to and from `NumPy arrays`
- NumPy arrays are powerful `N dimensional` array objects.
- NumPy have sophisticated `broadcasting` functions.
- It makes processing for images faster.
- Every NumPy array is a grid of elements of the same type.

```
Image Processing
```
- `Extracting` infromation from image and `enhancing` the image quality.
- Computers visualize images as a `matrix`
- Each element in matrix is a `pixel`
- `OpenCV` reads the image in channel order `BGR` format but `Matplotlib` and other visualization tools read in `RGB` order.
- Each pixel have color information composed of `3 channels` (B G R) containing numbers from `0` to `255`
- Each pixel of `matrix` represents the **intensity** of an color.
- Each channel need `8 bits` for storage therefore it become `24 bits` for each pixel.
- Some images need to be converted to `Grayscale` or `Binary` before applying any image processing.
- `Blending` : Overlaying images on top of each other by adjusting dimensions and opacity.
- `Thresholding` : Segmenting or dividing images into different parts.
- `Binary Thresholding` : Value below threshold will be shifted to `0` else `255`
- `Bianry Inverse Thresholding` : Value below threshold will be shifted to `255` else `0`
- `Truncation Thresholding` : Value below threshold will be shifted to `threshold value` else `remain same`
- `Threshold To Zero` : Value below threshold will `0` else `remain same`
- `Threshold To Zero Inverse` : Value below threshold will `remain same` else `0`
- `Blurring` : Adding noise 
- `Smoothing` : Removing noise to focus more on general details of the images.
- `Edge Detection` : Detect edged in high resolution images without bluring.
- `Gamma Correction` : Makes images `brighter` or `darker` based on choosen gamma value ( Lower gamma value : Brighter images )
```python
print(Image.shape)

(340, 540, 3) : (height, width, channel)
340 represents rows | height 
540 represents columns | width
3 represents channels.
```

### Images are converted to and from `NumPy Array`

### Storage Requirements

Image Type | Storage (Bits Per Pixel) | Channel
:--- | :---: | :---:
Binary | `1` | 
B/W | `8` | `1`
Grayscale | `8` | `1`
Color | `24` | `3`

Color | Channel
:---: | :---:
`B` | `0`
`G` | `1`
`R` | `2`

### `Pixel`
- Basic fundamental `unit` of an image. 
- Multiple pixels arranged in `rows` and `columns` forms an image.
- Binary, black and white, grayscale, RGB color image.

### `Black & White` and `Greyscale` images are `different`
- `B/W` is only composed with either `black` or `white`
- `Greyscale` is combination of different `shades` of black and white.

### Image Formats

- `HSV`
- `HLS`

```
Applications 
```
1. `Autonomous` self driving cars : Detect objects and humans infront of car, reverse parking.
2. Facial recognition : Attendance, FB friend recognition.
3. `AR` : Augmented Reality and `VR` : Virtual Reality
4. Health care : X Ray and MRI scan.
5. Video motion analysis : Detect face, Object in video.
6. Image `segmentation` : Camera detects the multiple faces in a group selfie.
7. Scene `reconstruction` : 3D model creation in architecture, room interior.
8. Image `restoration` : Filtering blur images and removing noise.

`DNN` is OpenCV's deep learning module.

The below step you will find in many articles and videos, It simply represents :
- To `mirror` the image you simply need to reverse either the `x` or `y` coordinates.
```python
# Trick to reverse BGR to RGB and keep x and y as it is (One liner code)
image[:, :, ::-1] 

# You can also the method :
cv2.cvtColor(src=image, code=cv2.COLOR_BGR2RGB)
```
