# Deep Learning

`Tensors` are N dimensional array.

`Scalar` | `Vector` | `Matrix` | `Tensors`
:---: | :---: | :---: | :---:
`1` | `[1, 2, 3]` | `[[1, 2, 3],[4, 5, 6],[7, 8, 9]]` | `[[[1, 2],[3, 4]],[[5, 6],[7, 8]]]`

Tensors make it very convenient to feed in sets of images into our model - `(I, H, W, C)`
- `I` : Images
- `H` : Height of images in pixels.
- `W` : Width of images in pixels.
- `C` : Color channels (`1` : Grayscale, `3` : RGB)

### `DNN` : Densely Connected Neural Network
Each and every neuron in one layer is connected to every other neuron in the next layer.

### `CNN` :  Convolutional Neural Network
Each `unit` is connected to a smaller number of nearby units in next layer.
