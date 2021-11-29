# `Super Resolution` in OpenCV

- `Super resolution` refers to the process of `upscaling` or `improving` the details of the image.
- When increasing the `dimensions` of an image, extra pixels need to be `interpolated` (alter or insert something new)
- Basic image processing do not give good results as they do not take the surrounding in context while scaling up.
- `Deep learning` gives better result in terms of high resolution image.
- The original high resolution image shows the best details when `zoomed in`
- The other images are achieved after `reconstruction` (using various `super resolution` methods)

`OpenCV` currently offers `4` deep learning algorithms for `upscaling` images.
- Images are `upscaled` using various standard resize operations in OpenCV using `Bicubic Interpolation` method.

1. `EDSR` : Enhanced Deep Residual Networks for Single Image Super Resolution
2. `ESPCN` : Real Time Single Image Super Resolution using an Efficient Sub Pixel Convolutionl Neural Network. 
3. `FSRCNN` : Accelerating the Super Resolution Convolutional Neural Network.
4. `LapSRN` : Fast and Accurate Image Super Resolution with Deep Laplacian Pyramid Networks.

- `EDSR`, `ESPCN` and `FSRCNN` offer an upscale ratio of `2x` `3x` and `4x` times.
- While `LapSRN` offer `2x`, `4x` and `8x` times the original size.
- `opencv-contrib-python` is important for Super Resolution.
- Super Resolution is present inside the module `dnn_superres` Deep Neural Network based Super Resolution.
```python
# Install module
!pip install opencv-contrib-python

# Import library
import cv2

cv2.dnn_superres()
```
- Prefer creating a `virtual environment` and install `opencv-contrib-python` inside that to avoid dependency issues.

