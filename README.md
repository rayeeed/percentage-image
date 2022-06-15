# get percentage values of the objects in an image
This code uses MIT CSAIL Computer Vision's image segmentation algorithm to extract percentage values of 150 objects in an image.

The original segmentation algorithm is trained on ADE20K dataset and it can mask 150 different objects accurately. However, I needed the percentages of those 150 objects in a tabular format. Hence I changed the code accordingly. The original segmentation algorithm individually identifies each pixel and applies a masking layer accordingly. So all I had to do was to create a function that will count the number of pixels of every object, count the total number of pixels in the image and yield the percentage value of each objects. Rest of the notebook represents that data in a tabular way. Also, for my project I needed 4 images of same grid be averaged, second dataframe df is created for that purpose.

In this code, my image naming format was grid-(some number)-(some number).jpg. If your images have different naming format, please change the code accordingly. In the second cell of the notebook, frameImage() function is defined, where you can change the naming format.
I stored my images in drive before analyzing them. Adjust the directory as you need.

This is my first github upload, so I am not sure if I am messing anything up. Any guidance will be appreciated!
