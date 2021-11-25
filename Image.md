### How computers handle `images` ?

- Let's imagine we have a simple image of a handwritten number.
- Each single digit image can be represented as an `array`
- e.g Single digit image will be represented by `28` x `28` pixels.
- Pixels are represented as a value between `0` and `1` (B/W and Greyscale)
- Default images have values between `0` and `255`
- `0` : No Color Value.
- `255` : Full Color.
- The range `0` to `255` has to do with how computers store `8 bit` numbers.
- `Color` images can be represented as a combination of `Blue`, `Green` and `Red`
- Each color channel will have `intensity` values between `0` and `255`
- The `shape` of the color array has `3` dimensions. (1, 2, 3)
- `1` : Pixel Height | NumPy Row
- `2` : Pixel Width | NumPy Column
- `3` : 3 Color Channels (`R`, `G` and `B`) in OpenCV it's (`B`, `G` and `R`)

### `HSL` and `HSV`
- `HSL` : Hue, Saturation, Lightness.
- `HSV` : Hue, Saturation, Value.
- `HSL` and `HSV` are more closely aligned with the way human vision actually perceives color.

