# `Super Resolution` in OpenCV

- `Super resolution` refers to the process of `upscaling` or `improving` the details of the image.
- A class to `upscale` images via `CNN : Convolutional Neural Network`
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

- `EDSR`, `ESPCN` and `FSRCNN` offer an upscale ratio of `2x` `3x` and `4x` 
- While `LapSRN` offer `2x`, `4x` and `8x` the original size.
- `opencv-contrib-python` is important for Super Resolution.
- Super Resolution is present inside the module `dnn_superres` Deep Neural Network based Super Resolution.

Important `Parameter`
1. `algo` : String containing one of desired models ( `'EDSR'`, `'ESPCN'`, `'FSRCNN'` or `'LapSRN'`  )
2. `scale` : Integer specifying the `upscale factor`

### `.pb` : `Protobuf`
- The `protobuf` file contains the `graph` definition as well as the `weights` of the model.

```python
# Install module
!pip install opencv-contrib-python

# Import library
import cv2

cv2.dnn_superres()
```
- Prefer creating a `virtual environment` and install `opencv-contrib-python` inside that to avoid dependency issues.

### `Application`

1. `Medical Imaging`
- Improving the quality of `X Rays`, `CT Scans`, etc.
- Highlight important details about the anatomical and functional information of the human body.
- Improving and enhancing medical images (helps in highlighting critical blockage or tumours)

2. `Multimedia` 
- Image and video processing applications, super resolution can convert hazy frames from a cell phone video into clearly readable image.

3. `Biometric Identification`
- Enhancement for face, fingerprint and iris images.
- The shape, structure and texture are  greatly enhanced which helps in distinctly identifying a biometric print.

4. `Remote Sensing`
- Remote sensing and Satellite imaging has been developed for decades.
- Infact the idea of super resolution was motivated by the need of better quality resolution of `landsat remote sensing` images.

5. `Astronomical Imaging`
- Improving the resolution of astronomical pictures help in focusing on tiny details that could turn out into discovery.

6. `Surveillance Imaging`
- Traffic surveillance and security system play a very important role in maintaining civilian safety.

### `Conclusion`
- `EDSR` comfortably gives the best result out of `4` methods, however it is slow and cannot be used for real time applications.
- `ESPCN` and `FSRCNN` are go to methods if real time performance is desired and have almost identical performance.
- `8x` upscaling model of `LapSRN` performs better in most situations.
- Although none of these methods can match the traditional `bicubic` method `speed`, they certainly give better results.
