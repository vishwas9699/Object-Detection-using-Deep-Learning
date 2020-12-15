# Introduction to Tensorflow Object Detection API

Convolutional Neural Networks have revolutionalized Pattern Recognition in last decades. As a result, CNNs are currently used for varous applications such as Object Detection and Image Recognition.

The TensorFlow object detection API is a software framework used for object detection tasks. Tensorflow Object Detection API and other similar APIs (Keras RCNN, YOLO) uses pre trained CNNs inside the framworks for predictions. Most of those pretrained models are trained using, the COCO dataset, the KITTI dataset, and the Open Images Dataset. These models are trained to detect some fixed type of categories of objects such as, persons, cars, dog, tooth brush and etc. If you want to detect custom objects you can retrain those models using your own datasets.

## CNN models used in Tensorflow Object Detection API

<img src="https://github.com/vishwas9699/Object-Detection-using-Deep-Learning/blob/main/README%20resource/0.png">

### mAP (mean Average Precision)

AP (Average precision) is a popular metric in measuring the accuracy of object detectors like Faster R-CNN, SSD. Average precision computes the average precision value for recall value over 0 to 1

## How Object Detection is done 

1. Generates the small segments in the input image
<img src="https://github.com/vishwas9699/Object-Detection-using-Deep-Learning/blob/main/README%20resource/1.png">

2. Feature extraction is carried out for each segmented rectangular area to predict whether the rectangle contains an valid object.
<img src="https://github.com/vishwas9699/Object-Detection-using-Deep-Learning/blob/main/README%20resource/2.png">

3. Overlapping boxes are combined into a single bounding rectangle (Non Maximum Supression)
<img src="https://github.com/vishwas9699/Object-Detection-using-Deep-Learning/blob/main/README%20resource/3.png">

## SSD Mobile Net

<img src="https://github.com/vishwas9699/Object-Detection-using-Deep-Learning/blob/main/README%20resource/4.png">

### Input

300x300 color Image (3@300x300)

### Outputs

SSD Mobile Net output the category of the detected objects and coordinates of there bounding rectangles offset (x,y,w,h)

<img src="https://github.com/vishwas9699/Object-Detection-using-Deep-Learning/blob/main/README%20resource/5.png">[#]