# Detection and Decoding of Barcode using Image Processing techniques

# Algorithm used for detecting :-
 ![App Screenshot](https://github.com/bhim4078652/Detection-and-Decoding-of-Barcode-using-Image-Processing-techniques/blob/main/pr1.jpg)
 
## step 1 : conversion to gray scale image
- colored image contains 3 channel that is three 2d matrices one for red , one for green and another for blue color.
- gray scaling converts 3 channel image into 1 channel image which is one of the important step in the edge detection.

 ![App Screenshot](https://github.com/bhim4078652/Detection-and-Decoding-of-Barcode-using-Image-Processing-techniques/blob/main/pr2.jpg)

## step 2 : calculating gradient in both x and y direction
- We use gradients for detecting edges in images, which allows us to find contours and outlines of objects in images.
- Gradient of the image defines the different order of derivative of intensity versus pixel number plot.
- In our project we have used sobel high pass filter which finds approximate first order derivative using sobel operators which are nothing but kernels which various       size and we have taken kernel size of 3 which gives optimum result.
- Sobel operators is a joint Gausssian smoothing plus differentiation operation, so it is more resistant to noise. 
- cv2.Sobel(gray, ddepth=ddepth, dx=1, dy=0, ksize=-1).
- dx=1 implies derivative in x direction keeping y constant and ksize=-1 implies the kernel size of 3 which is by default and ddpeth is desired depth of output.
- We could also use the Scharr kernel instead of the Sobel kernel which may give us better approximations to the gradient and the function parameters for Scharr gradient   remains same.





