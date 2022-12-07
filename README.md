# Image-Processing-UPES

### Task 1

1.	Image resizing is a widely used operation in image processing. Either for scaling up or for scaling down, we use interpolation to find the corresponding pixel intensity in the resulting image. Choice of interpolation method is important as it directly affects the quality of the resulting image. The following interpolation methods were mentioned in class: <br>

     • Nearest neighbour<br>
     • Bilinear <br>
     • Bicubic <br>

    If you look at PILLOWS reference page you can see that the resize() function has predefined resampling functions: <br>

    • PIL.Image.NEAREST <br>
    • PIL.Image.BILINEAR <br>
    • PIL.Image.BICUBIC <br>
    • PIL.Image.LANCZOS <br>

      LANCZOS is a more sophisticated method which gives better results compared to first three methods. If you're interested search the internet for more details on LANCZOS Resampling Method. <br>

     For this question, you will implement a jupyter notebook script and it will perform these operations :

    Ques 1. Read color version of the image "lena.png", Convert colored lena image to grayscale image. <br>
    Ques 2. Resize (scale down) the grayscale lena image to half its original size. Then, resize (scale up) it up back to the original size using resize() with PIL.Image.NEAREST <br>
    Ques3. Resize (scale down) the grayscale lena image to half its original size. Then, resize (scale up) it up back to the original size using resize() with PIL.Image.BILINEAR <br>
    Ques4. Resize (scale down) the grayscale lena image to half its original size. Then, resize (scale up) it up back to the original size using resize() with PIL.Image.BICUBIC <br>
    Ques5. Your script should display the results as follows using matplotlib along with the PSNR values w.r.t original image below the result image
-----------------------

2.	Ques1. Define a generic function (ChSwap) that takes a color image as input and returns the corresponding output image in which the R,G,B channels are swapped as follows: <br>
o Splits the input image into R, G, B Channels o Red (Out) = Blue (In)<br>
o Green (Out) = Red (In) o Blue (Out) = Green(In) <br>
o Combine the new channels to create the new image and return <br>

     Ques2. Read color version of the image "Lenna.png”.<br>
     Ques3. Use function ChSwap to create a color band swapped version of lena  <br>
     Ques4. Using matplotlib plot, display the original and new images side-by-side. <br>
 
 ---------------------------

3.	Ques1. We have discussed intensity transformation functions in detail in class and you have gained necessary implementation skills from Lab1. Now, let’s apply them to a real life challenge! <br>

     Ques2. Although not very common among us Indians, red-eye effect is a common phenomenon in flash photography where pupils in the eyes appear red! Automatic Redeye Detection and Correction Algorithms are now very common in most cameras and cell phones!! (Due to the inherent complexity, we will not deal with automatic detection aspect now, but will only work on correction) <br>

     Ques3. Come up with your own red-eye correction algorithm (RedEyeRemoval) using piece-wise intensity transformations! (Don’t worry if other parts of the image with red color get distorted!) <br>
     
     Ques4. Two important aspect of this algorithm are (1) Figuring out the range of intensities to modify (2) Deciding on what the modified intensity values should be! <br>
     
     Ques5. Four sample images with red eyes are provided with this lab. Your function, RedEyeRemoval, should take an input image and display/output the corrected image. Using matplotlib plot, display the original and new images side-by-side. (Test your algorithm on all the sample images. <br>
     
     -----------------------------------

### Task - 2


- You have to take an image of your face. Make sure you're wearing clear spectacles so that more edges are visible. 
- There should be three images(one clear image, one with gaussian noise and one with salt and pepper noise)
- Perform 5 edge detection techniques on these three images <br>
1. Prewitt Edge Detection <br>
2. Sobel Edge Detection <br>
3. Laplacian Edge Detection <br>
4. Canny Edge Detection <br>
5. Robert Edge Detection <br>
- Perform Thresholding Technique <br>
1. Simple/Binary Thresholding <br>
2. Mean Adaptive Thresholding <br> 
3. Gaussian Adaptive Thresholding <br>
4. Ostu's Thresholding <bn>

-----------------------------------
