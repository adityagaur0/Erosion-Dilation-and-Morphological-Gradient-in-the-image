# Erosion-Dilation-and-Morphological-Gradient-in-the-image

**Morphological operations** are a set of operations that process images based on shapes. They apply a structuring element to an input image and generate an output image. 
The most basic morphological operations are two: 
> ErosionDilation 

*Basics of Erosion:*
Erodes away the boundaries of the foreground object
Used to diminish the features of an image.
Working of erosion: 

A kernel(a matrix of odd size(3,5,7) is convolved with the image.
A pixel in the original image (either 1 or 0) will be considered 1 only if all the pixels under the kernel are 1, otherwise, it is eroded (made to zero).
Thus all the pixels near the boundary will be discarded depending upon the size of the kernel.
So the thickness or size of the foreground object decreases or simply the white region decreases in the image.
Basics of dilation: 

Increases the object area
Used to accentuate features
Working of dilation:

A kernel(a matrix of odd size(3,5,7) is convolved with the image
A pixel element in the original image is ‘1’ if at least one pixel under the kernel is ‘1’.
It increases the white region in the image or the size of the foreground object increases 
