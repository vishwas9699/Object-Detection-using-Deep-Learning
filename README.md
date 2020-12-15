# Introduction to Tensorflow Object Detection API

Convolutional Neural Networks have revolutionalized Pattern Recognition in last decades. As a result, CNNs are currently used for varous applications such as Object Detection and Image Recognition.

The TensorFlow object detection API is a software framework used for object detection tasks. Tensorflow Object Detection API and other similar APIs (Keras RCNN, YOLO) uses pre trained CNNs inside the framworks for predictions. Most of those pretrained models are trained using, the COCO dataset, the KITTI dataset, and the Open Images Dataset. These models are trained to detect some fixed type of categories of objects such as, persons, cars, dog, tooth brush and etc. If you want to detect custom objects you can retrain those models using your own datasets.

## CNN models used in Tensorflow Object Detection API

![Models used in Tensorflow Object Detection API](https://cdn-images-1.medium.com/max/800/1*-EyxSs2OiyWm-E6MSpSJiA.png)

### mAP (mean Average Precision)

AP (Average precision) is a popular metric in measuring the accuracy of object detectors like Faster R-CNN, SSD. Average precision computes the average precision value for recall value over 0 to 1

## How Object Detection is done 

1. Generates the small segments in the input image

![image.png](attachment:image.png)
