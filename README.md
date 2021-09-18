# object_detection

![Clean and Jerk](https://github.com/Ortgies/object_detection/blob/main/graphics/video_3_f%20.gif)


# Data collection
I retrieved three videos of olympic weight lifting from Youtube. <br>
The first two were used to generate training images. I took one frame each second and used labelIMG to generate bounding boxes for the bar. These were saved in XML files based on the Pascal VOC format. <br>
The third video was only used to test the detection model.

# Model training
I used the custom object detection algorithm from ImageAi to train a model. <br>
210 frames were used for training and 50 frames were used for valuation. The model has a mean average precision of 99.90%. <br>
Since the current version imageAi requires older CUDA drivers that do not support my graphics card, the training was done in Google Colab.

# Results
