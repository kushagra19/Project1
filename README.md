<!-- background: #e4dadf-->
<!-- color: #774c43 -->
<!-- font: univers -->

<h1 align="center">
<span style = "color: #FFC300">
Project1
</span>
</h1>

* * *
## Introduction
 This repository consists of solutions to problems 3,4,5 of Project1.
***
## Installation
For installing the repository use the command below in your terminal.<br>
<code>
<blink>
    git clone https://github.com/kushagra19/Project1     
</blink>
</code>
***
## Description
### Problem3&4:
In this problem we were given data and we had to use the convex optimization problem obtained in the theory part of the assignment to solve for optimal solution and then reconstruct the given incomplete image using the soltution obtained.<br />
This folder consists of following files:
* **Problem3.ipynb** <br />
This file uses the data given in the Group1 folder in the assignment data link and uses compressive sensing to reconstruct the image.
For running the above code firstly follow installation steps to install the repository,then use the link: [Data for Problem3](https://drive.google.com/drive/folders/1yM_xa7rV1jwiqjGcIQCWKltziAsTWDjo?usp=sharing) to download data for the reconstruction.<br />
Once data is installed use the .ipynb file to obtain reconstructed image.<br />
 **NOTE:Update the path variable in the file to properly access data**.
* **complete.png**<br />
This is the completed image obtained after running the .ipynb file and kept in the repository for reference.

### Problem4&5:
In this part of the excercise we had to use our own sample RGB image and use the incomplete data to reconstruct the image and compare them.<br />
Steps to follow if you want to test on your own sample image.
* First follow the installation step to clone the repository.
* Now, use the problem4&5 folder to access code for testing on your own sample image.
The folder consists of:
  * create_random_indices.ipynb
  * combine_comp.ipynb
  * Sample images
  * img.Png
  * R
  * G
  * B
* Select a 100X100 pixel image (otherwise PC might crash) and use create_random_indices.ipynb to select randomly some pixels which you want to retain in incomplete image.
* Folders R,G,B are used to do reconstruction separately for Red,Green and Blue components respectively.Each of them contains two files create_data.ipynb and recons.ipynb.
* One by one use create data for obtaining incomplete matrices to be used in recons.ipynb to reconstruct image.
* Firstly create data and then use recons for each R,G,B for obtaing reconstructed image of that particular component.
* Check the R,G,B folders once execution complete.If a new folder 'data for assignment' has been created and file with extension .npy is created then execution is successful.
* Now for the final step use comine_comp.ipynb to combine all components into one image and compare with the final image.
* Sample_images contains reconstructed images:
  * reconstruct_0.4.png - reconstructed image when corruption 40%
  * reconstruct_0.7.png - reconstructed image when corruption 70%
* img.png is the sample image used for reconstruction.

**NOTE:Change path variable according to your files in order for the code to work properly.**
