<h1 style="text-align:center">

  <br>

  Safety Helmet Detection using Yolov5s model 

</h1>

<h3 style="text-align:center">

  Computer Vision / Deep Learning  Project 

</h3>

<div style="text-align:center">

  <h4>

   <a href="#Introduction">Introduction</a> | <a href="#Demo">Demo</a> | <a href="#Helmet Detection">Helmet Detection</a> | <a href="#Helmet Tracking">Helmet Tracking</a> | <a href="#References">References</a> | <a href="#Contribution">Contribution</a>

  </h4>

</div>

<br>

 

## Introduction

The primary purpose of this project is to detect and track helmets of construction workers in industry sites to reduce the risk of injuries and ensure their safety using a Deep learning model which is Yolov5s with PyTorch, to detect whether or not workers are wearing PPE
helmets during the experiment.

This repository is organised to make it reproductible, with Colab notebook and the necessary configuration files are made available.
the first part of the notebook is implemented to detect helmets using the Harvard Data-verse shared by Northeastern University-China dataset which contained 7063 images annotated online with RoboFlow. and the second part of the colab notebok is to track helmets using internet videos to test the yolov5s model with the best weight. The machine learning library PyTorch is also used in this process and it includes: 

1. Data processing 
2. Model Training 
3. Model evaluation 
4. Model saving 

## Demo

The following images presents different scenarios of workers in the construction sites. We tagged the head parts of each worker in the photographs with a bounding box and the label “helmet,” or if they were not wearing a helmet, then labelled “head”.
<img src="/images/workers.png">
And this is a video that shows the prediction results of yolov5s model. 
https://drive.google.com/file/d/1Rk4eQ19BabCQhamG_WKxXKXLCB8WtN3j/view?usp=share_link 

## Helmet Detection

The purpose of Helmet detection is after receiving an image; we need to
alert workers to wear their helmets, we used only those frames for YOLOv5s with an image size of 640 for better extraction. We created a data.yaml as a configuration file to train yolov5s model with 2 classes : helmet and head. The YOLOv5 is trained to learn how to put labels
and bounding boxes on the new images given to it. the number of epochs we trained with is 30 and batch 32.     


## Helmet Tracking

The purpose is to tracking helmets in videos using yolov5s model with best weights. If workers are not wearing helmets, automatic detection of the head alerts them as well as their monitors that their lives are in danger. 
 

## References 

- Papers and Dataset:

  - <a href="https://ieeexplore.ieee.org/document/9362711?fbclid=IwAR1X-9bqVV5CiVV3rChLpzAXlr6b9L6nhQ9WPiGA6wcd7RmBzsN8K7f1vsA">Safety Helmet Detection Based on YOLOv5</a>

  - <a href="https://universe.roboflow.com/joseph-nelson/hard-hat-workers/browse?queryText=&pageSize=50&startingIndex=0&browseQuery=true">Hard Hat Workers</a>

- Codes and Tools:

  - <a href="https://github.com/ultralytics/yolov5">Yolov5 model</a>

  - <a href="https://github.com/Mrinal18/NFL_Kaggle">tracking with yolov5 model</a>

  

## Contribution

This project was developed as part of our computer vision and deep learning  project at Sup'Com.

<a href="https://github.com/Malek-1">Malek Abbes</a>

<a href="https://github.com/Ines38">Ines Bougheriw</a>