# object_detection

![Clean and Jerk](https://github.com/Ortgies/object_detection/blob/main/graphics/video_1_f.gif)


# Data collection
I retrieved three videos of olympic weight lifting from Youtube. <br>
The first two were used to generate training images. I took one frame each second and used labelIMG to generate bounding boxes for the bar. These were saved in XML files based on the Pascal VOC format. <br>
The third video was only used to test the detection model.

# Model training
I used the custom object detection algorithm from ImageAi to train a model. <br>
210 frames were used for training and 50 frames were used for valuation. The model has a mean average precision of 99.90%. <br>
Since the current version imageAi requires older CUDA drivers that do not support my graphics card, the training was done in Google Colab.

# Results
Detection of the bar works quite well, considering that training was done with just 200 pictures.<br>
There are some frames where the model has difficulty following the bar, but with some interpolation the bar path can still be plotted on a graph. <br>
The following are a few example videos with the corresponding bar baths. Note: In the videos the bar position starts at 225mm, half the radius of an olympic plate. <br>

**Clean and Jerk 1**<br>
<img src="https://github.com/Ortgies/object_detection/blob/main/graphics/video_3_f%20.gif" width="480" height="270"/> <img src="https://github.com/Ortgies/object_detection/blob/main/graphics/3_height.png" width="350" height="270"/> 

**Clean and Jerk 2**<br>
<img src="https://github.com/Ortgies/object_detection/blob/main/graphics/video_4_f.gif" width="480" height="270"/><img src="https://github.com/Ortgies/object_detection/blob/main/graphics/4_height.png" width="350" height="270"/> 

**Clean and Jerk fail** <br>
<img src="https://github.com/Ortgies/object_detection/blob/main/graphics/video_5_f.gif" width="480" height="270"/><img src="https://github.com/Ortgies/object_detection/blob/main/graphics/5_height.png" width="350" height="270"/> 

**Snatch** <br>
<img src="https://github.com/Ortgies/object_detection/blob/main/graphics/video_6_f.gif" width="480" height="270"/><img src="https://github.com/Ortgies/object_detection/blob/main/graphics/6_height.png" width="350" height="270"/> 

**Snatch fail** <br>
<img src="https://github.com/Ortgies/object_detection/blob/main/graphics/video_7_f.gif" width="480" height="270"/><img src="https://github.com/Ortgies/object_detection/blob/main/graphics/7_height.png" width="350" height="270"/> 
