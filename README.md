# object-detection

For implementation we will going to use python as a programming language.
And for ordering this rectangle and text data we will be using opencv
For object detection and image classification we will be going to use pre-trained deep learning architecture based on tensorflow
Using opencv we will load already pretrained tensorflow frozen models.
-----------------------------------------------------------------------------------------------------------------------------------
Before dive into implemtation I would like to explain concept that used in our project.
Image classification, object detection and image segmentation are the three important concept to implement our project
For object detection from an image we will going to use (singleshot multibox detector) which divides image into small patches, based on salient features it joins all the patches and ask the classifier like mobilenet to classify this image combination of two algorithm like SSD-mobilenetv2, SSD-mobilenetv3 for better object detection. And we will use coco as a dataset which have 80 classes.
Image segmentation is to classify rather than classifying object it is to classify each pixel based on salient features foreground and background is segmented.
------------------------------------------------------------------------------------------------------------------------------------
Let’s dive into the implementation part
Tools that we used:
Anaconda: it has package of multiple libraries and IDE.
We will use Jupiter notebook as an IDE.
And also we will use opencv as a library. To install opencv just type pip install opencv-python in anaconda prompt.
-------------------------------------------------------------------------------------------------------------------------------------- 
First we have to import cv2
Second tool that we used is matplotlib
Now we have to give path of configuration file and frozen file
To load Tensorflow pre trained model we have to right this command i.e.
Now I have written the code for loading the label 
This ssd model have already some configuration to setup those configuration I have written this command.
 
Now let’s read an image
This command line is used to read an image.
And then I have plot it using matplotlib library.
Classindex, confidence and bbox help us to show the output and this is threshold based on the accuracy we want.
This is the code for flatten the classindex and confidence and for styling purpose.
Now I have to plot again to see the output.
This is the final output it successfully detect an no of object and classify accrding to labels.



