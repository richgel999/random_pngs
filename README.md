# random_pngs
A collection of 2,943 random PNG test files for validation and fuzzing purposes, generating with [lodepng](https://lodev.org/lodepng/). The filename format is:

```
sprintf(filename, "rand_%u_%u_%u_%u_%u_%u_%u.png", width, height, bit_depth, ct, has_key, uses_pal_alpha, interlace_method);
```

width/height ranges between [1,32]

bit_depth is 1, 2, 4, 8, or 16

ct is the PNG color type: 0, 2, 3, 4, or 6

has_key is 1 if the PNG uses a TRNS chunk for colorkey transparency

uses_pal_alpha is 1 if a palettized PNG uses alpha transparency

interlace_method is 1 if the PNG uses adam7 interlacing

The pixel data is entirely psuedo-random.
