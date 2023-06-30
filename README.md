# Image Unblurring using Fast Fourier Transform and Wiener Deconvolution
Applied Fast Fourier Transforms (FFT) for image processing, particularly in image blurring and unblurring. Through manipulating an image in the frequency domain using FFT, we can blur the image and unblur it to a certain extent.

Explored the process of blurring and unblurring grayscale and RGB images. While we were able to unblur the blurred image directly, the restoration was less effective when working with loaded blurred images. This was due to information loss and noise introduced during the save and load process, as well as during normalization of the pixel values.

To overcome these limitations, I utilized Wiener Deconvolution, a more advanced technique for image restoration. It reduces the noise amplification during fourier transforms, resulting in a more effective restoration of the loaded blurred images.

Explored the condition where the Point Spread Function is not analytic but instead has to be derived from blurred and filtered images. Using this non-analytic PSF, we could blur and unblur our target images even better. In this case, the Wiener Deconvolution still outperfoms the standard method.
