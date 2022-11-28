# Image-Processing-UPES

### Programmin Assignment 1

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
