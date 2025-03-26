# Image-Processing
Various functions for image analysis, such as resampling, filtering, and segmentation.

Functions written by Eleni Christoforidou in MATLAB R2022b.

**ImageResample:** This function takes as input an [MxN] image matrix img that we would like to resample and a [2x1] vector dim, which contains the desired size of the resampled image. The function outputs img_resamp, the resampled version of image with datatype double and dimensions dim.

**SobelMagnitude:** This function computes the magnitude of Sobel filter responses for the input image 'img' using the horizontal and vertical Sobel filters. The function outputs 'edge_mag', the magnitude of the filter responses.

**OtsuThreshold:** This function takes as input an [MxN] uint8 image matrix img, and outputs the Otsu thresholded binary image in  [MxN] matrix msk, as well as the integer threshold thrsh used to make msk.

**edgy:** This function takes an original image input, and produces a processed image. Both the input and the output argument are grayscale images, that is, matrices of uint8 values. Note that the output has two fewer rows and columns than the input since the pixels in the first and last columns and rows do not have enough neighbors for the required computation. The function uses the Sobel operator. An example input image is provided.

_Example input and output:_

![example image](https://github.com/eleni-chr/Image-Processing/blob/master/example.png)
