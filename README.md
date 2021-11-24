### Open Computer Vision

```python
pip install cv2
```

- Computers gain high level understanding from digital `image` and `video`
- Understand and automate the task of `human visual system`
- `Detecting` and `labelling` image or object has surpassed humans.
- `Faster` than human reaction and `99% Accuracy`
- High amount of visual data i.e images and videos with high processing capabilities.

### Image Processing
- `Extracting` infromation from image and `enhancing` the image quality.
- Computers visualize images as a `matrix`
- Each element in matrix is a `pixel`
- Each pixel have color information composed of `3 channels` (R G B) containing numbers from `0` to `255`
- Each pixel of `matrix` represents the **intensity** of an color.
- Each channel need `8 bits` for storage therefore it become `24 bits` for each pixel.

### Images are converted to and from `NumPy Array`

### Storage Requirements

1. Binary : `1 Bit` per pixel.
2. Black and White : `8 Bits` per pixel | `1 Channel`
3. Grayscale : `8 Bits` per pixel | `1 Channel`
4. Color : `24 Bits` per pixel | `3 Channels`

### Pixel
- Basic fundamental unit of an image. 
- Multiple pixels arranged in `rows` and `columns` forms an image.
- Binary, black and white, grayscale, RGB color image.

> Black and White and Greyscale Images are **Different**
- Black and White is only Composed with Black or White
- Grayscale is combination of Different Grades of Black and White.

- **Binary** need `1 Bit Per Pixel` for Storage and **Black** and **White** needs `8 Bits Per Pixel` for **Storage**.
- Black and White will be **Dense** and shall render **Better Quality**.

### Applications 
1. Self Driving Cars (Detect Objects and Humans infront of Car, Reverse Parking)
2. Facial Recognition (Attendance, FB Friend Recognition)
3. Augmented Reality and Virtual Reality
4. Health Care (X Ray and MRI Scan)
5. Video Motion Analysis (Detect Face, Object in Video)
6. Image Segmentation (Camera Detects the Multiple Faces in a Group Selfie)
7. Scene Reconstruction (3D Model Creation in Architecture)
8. Image Restoration (Filtering Blur Images and Removing Noise)
