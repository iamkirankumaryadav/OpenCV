# Deep Learning

### `Tensors` are N dimensional array.

`Scalar` | `Vector` | `Matrix` | `Tensors`
:---: | :---: | :---: | :---:
`1` | `[1, 2, 3]` | `[[1, 2, 3],[4, 5, 6],[7, 8, 9]]` | `[[[1, 2],[3, 4]],[[5, 6],[7, 8]]]`

### `I, H, W, C`
Tensors make it very convenient to feed in sets of images into our model - `(I, H, W, C)`
- `I` : Images
- `H` : Height of images in pixels.
- `W` : Width of images in pixels.
- `C` : Color channels (`1` : Grayscale, `3` : RGB)

### `DNN` : Densely Connected Neural Network
Each and every neuron in one layer is connected to every other neuron in the next layer.

### `CNN` :  Convolutional Neural Network
- Each `unit` is connected to a smaller number of nearby units in next layer.
- Pixels nearby to each other are much more `correlated` to each other for imaged detection.
- Each `CNN` layer looks at an increasingly larger part of the image.
- `CNN` also helps with `regularization`, limiting the search of `weights` to the size of convolution.

### How the `Convolutional Neural Network` relates to `Image Recognition`.
1. We start with the `input layer`, the image itself.
2. `Convolutional layers` are also connected to `pixels` in their respective fields.
3. We add a `padding` of `zeros` around the image so that we do not miss the `outer edge` of image.
