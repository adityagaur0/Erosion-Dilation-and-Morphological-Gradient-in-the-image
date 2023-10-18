# Erosion-Dilation-and-Morphological-Gradient-in-the-image

Morphological operations are a set of operations that process images based on shapes. They apply a structuring element to an input image and generate an output image. 
The most basic morphological operations are two: 
### ***Erosion***

<img width="513" alt="Screenshot 2023-10-18 at 1 09 47 PM" src="https://github.com/adityagaur0/Erosion-Dilation-and-Morphological-Gradient-in-the-image/assets/112656570/d1cbe6db-29b0-4db8-9c8b-540852d5e530">

  *Basics of Erosion:*
  1. Erodes away the boundaries of the foreground object.
  2. Used to diminish the features of an image.
  
  *Working of erosion:*
  1. A kernel(a matrix of odd size(3,5,7) is convolved with the image.
  2. A pixel in the original image (either 1 or 0) will be considered 1 only if all the pixels under the kernel are 1, otherwise, it is eroded (made to zero).
  3. Thus all the pixels near the boundary will be discarded depending upon the size of the kernel.
  4. So the thickness or size of the foreground object decreases or simply the white region decreases in the image.
### ***Dilation***

<img width="511" alt="Screenshot 2023-10-18 at 1 07 10 PM" src="https://github.com/adityagaur0/Erosion-Dilation-and-Morphological-Gradient-in-the-image/assets/112656570/ebfe226b-aca1-4427-964e-772d8ee481cd">

  *Basics of dilation:*
  1. Increases the object area.
  2. Used to accentuate features.

  *Working of dilation:*
  1. A kernel(a matrix of odd size(3,5,7) is convolved with the image
  2. A pixel element in the original image is ‘1’ if at least one pixel under the kernel is ‘1’.
  3. It increases the white region in the image or the size of the foreground object increases 

## ***Apply some noise on the previous image by creating blobs on it. Then apply following operations on the noisy image:***

### **1. Opening**
An opening is an erosion followed by a dilation.

<img width="510" alt="Screenshot 2023-10-18 at 1 21 25 PM" src="https://github.com/adityagaur0/Erosion-Dilation-and-Morphological-Gradient-in-the-image/assets/112656570/ed69d7c6-cc8b-4b84-a504-64c12dd7ae29">


### **2. Closing**
The exact opposite to an opening would be a closing. A closing is a dilation followed by an erosion.

<img width="514" alt="Screenshot 2023-10-18 at 1 21 34 PM" src="https://github.com/adityagaur0/Erosion-Dilation-and-Morphological-Gradient-in-the-image/assets/112656570/e6344a26-57af-423a-a5ca-cc5345bc0e9f">

### **3. Morphological gradient**
A morphological gradient is the difference between a dilation and erosion.

<img width="509" alt="Screenshot 2023-10-18 at 1 21 53 PM" src="https://github.com/adityagaur0/Erosion-Dilation-and-Morphological-Gradient-in-the-image/assets/112656570/8cdeeff0-6c22-45ed-b758-700a41c42290">

### **4. Top hat/white hat and black hat**
A top hat (also known as a white hat) morphological operation is the difference between the original (grayscale/single channel) input image and the opening.

A top hat operation is used to reveal bright regions of an image on dark backgrounds.





