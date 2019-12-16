# Car Detection from Aerial Images with Faster R-CNN and YOLOv3

This repository contains files that were used to reproduce the following paper: https://arxiv.org/abs/1812.10968
Datasets were taken from https://github.com/aniskoubaa/car_detection_yolo_faster_rcnn_uvsc2019 and https://github.com/jekhor/aerial-cars-dataset

## To train Faster R-CNN follow the ipython notebook from the Faster R-CNN folder in Google Colab
![example_frcnn](https://github.com/kuvdaria/car_detection_paper_reproduction/blob/master/example_frcnn.jpg)

## To train YoloV3 on custom dataset use the following instructions
1) Download YoloV3 folder
2) Download yoloV3 NN weights from official website and convert the file into .h5 format
3) Prepare images and their labels in /Images/ and /Images/Labels/ folders respectively
4) Use oid_to_pascal_voc_xml.py to convert .txt labels into .xml labels
5) Use voc_to_YOLOv3.py to create single file with labels in acceptable by YoloV3 format
6) Modify train.py file specifying the path to CLASS and LABELS .txt files, batch size and number of epochs
7) For detaction use image_detect.py
