# 343-C-ImageManipulation

**Objectives:**
    - gaining comfort with C
    - understanding pointers

**Assignment:**

Images are just grids of pixels.  The values for the pixels are usually light intensities.  Colors are created by combining the intensity values for multiple colors - often red, green, and blue.  An image of a single pixel then, could be composed of three intensity values.  A 4x4 pixel image would have 16\*3 = 48 intensity values, and so on.

When the intensity values are written to a file, they are converted to one or more bytes depending on the encoding.  A perfectly white pixel is made of full intensities of red, blue, and green.  In the file, it may look like this:

``c
FF FF FF
```

Black, would be 

```c
00 00 00
```

Etc.  We can do image manipulation by loading the bytes from a file into memory, modifying the bytes, and rewriting the file.

For this assignment, you will write a program that will load an image, swap all the red and blue values, and rewrite the image.  If you do this correctly, you will turn

![Starting image](./inputImage.png)

into this:

![Ending image](./outputImage.png).
