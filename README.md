# CNN-Based_Adversarial_Embedding_for_Image_Steganography

Instructions to Run the Code 

1. Open "https://colab.research.google.com/" website and upload the 'ADV-EMB' python notebook file in colab

2. Conect the run time in colab with GPU

3. Check what GPU is alloted to your session using 'To find the GPU being used' cell
   the ranking order of the GPU's of google colab are K80 / T4 / P100 / V100 / A100 (low to high computation 
   power) 
   !! if you get K80 disconnect and delete runtime and reconnect to get T4 or above for better performace

4. If you have images in drive, mount your drive to 'content/drive' path using 'Mount google drive to colab'    
   cell 

5. Install all the dependencies by running the cell 'To install dependencies'

6. copy any image path and convert it to grey scale image using 'convert colour image to grey image' cell

7. To crop the grey image to (512x512) use the 'crop the image to (512x512) {final cover pics} cell

8. If you want to change the cropping measurements change it in code

9. Embed your message using 'Embed message in the image' cell , for that you need 
   --> imput_image_path = path of cover image
   --> msg_file_path    = create a text file and write the message in that file and give it's path 
   --> password         = add password to message 
   --> output_img_path  = path of the stego image that is going to be generated 

10. Extract the message that is embedded in the stego image using 'Extract the message from the image' cell,      
    for that you need 
   --> stego_img_path   = path of the stego image
   --> password         = password of the message
   --> output_msg_path  = a text file is generated where you can find your message

11. comparision of the both cover image and stego image using SSIM(The Structural Similarity Index Measure)
    using 'Compare the similarity between cover and stego images using SSIM(The structural similarity index    
    measure)' cell , for that you need 
   --> path1 = cover image path 
   --> path2 = stego image path


Note:

# This colab notebook uses Hill cost function for bitmap images(png) and J-UNIWARD for JPEG(jpg) images
