# Convolution Filters | `Kernels`

- Used with images for `blurring`, `sharpening`, `embossing`, `edge detection` and more.
- Helps in extracting specific features from image.
- Images are fundamentally `matrices`, where each digit represents `intensity` of light in that position.
- `Grayscale` image is represented by `1` matrix describing the intensity of light.
- `Colorful` image is represented by combination of `3` matrices, each representing intensity of `R`, `G` and `B`

![Emboss - Deboss](Image/EmbossDeboss.jpg)

- `Kernels` are typically `3 x 3` matrices.
- `Kernels` is overlapped with original image and slides (`stride`) from `top left` to `bottom right`.
- `Strides` : Number of steps the kernel moves or slides over an image matrix.
- Overlapping indices are `muliplied` and `added` to replace `center` value for each pixels in the image.
- `Corner` pixels of image is also included by using `padding`, `extending`, `wrapping`, `mirroring` and `cropping`
- Depending on filter values (Kernel), convolution can have a variety of effects.

![Kernel](Image/Kernel.png)

### `Sobel` Filters

- `Sobel` filters are best for detecting edges in an image (Especially for chessboard, bricks, etc)

`Horizontal` kernel :

![Horizontal Kernel](Image/HorizontalSobel.png)

`Vertical` kernel :

![Vertical Kernel](Image/VerticalSobel.png)
