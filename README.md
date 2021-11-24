### Open Computer Vision

```python
pip install cv2
```

- An open source computer vision and machine learning `library`.
- Contains over 2,500 optimized algorithms.
- Algorithms for Facial recognition, Object identification, Human action, Track movements,etc.

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

Image Type | Storage (Bits Per Pixel) | Channel
:--- | :---: | :---:
Binary | `1` | 
B/W | `8` | `1`
Grayscale | `8` | `1`
Color | `24` | `3`

### `Pixel`
- Basic fundamental `unit` of an image. 
- Multiple pixels arranged in `rows` and `columns` forms an image.
- Binary, black and white, grayscale, RGB color image.

### `Black & White` and `Greyscale` images are `different`
- `B/W` is only composed with either `black` or `white`
- `Greyscale` is combination of different `shades` of black and white.

### Applications 
1. `Autonomous` self driving cars : Detect objects and humans infront of car, reverse parking.
2. Facial recognition : Attendance, FB friend recognition.
3. `AR` : Augmented Reality and `VR` : Virtual Reality
4. Health care : X Ray and MRI scan.
5. Video motion analysis : Detect face, Object in video.
6. Image `segmentation` : Camera detects the multiple faces in a group selfie.
7. Scene `reconstruction` : 3D model creation in architecture, room interior.
8. Image `restoration` : Filtering blur images and removing noise.

`DNN` is OpenCV's deep learning module.
