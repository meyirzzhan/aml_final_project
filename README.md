# Object Detection and Segmentation Project

This project focuses on training and comparing two different architectures for object detection: YOLOv8 and Faster R-CNN. We use these models for recognizing road signs and speed limits.

## Technologies

- PyTorch
- Ultralytics YOLOv8
- Detectron2
- OpenCV



# DOWNLOAD DATASET
!curl -L "https://universe.roboflow.com/ds/MTYIKt7Lm7?key=vmsvtxlL9O" > roboflow.zip
!unzip roboflow.zip -d ./dataset

**use this commands to download dataset **


# USAGE

Launch Jupyter Notebook to start training and testing the models:

jupyter notebook faster_rcnn_for_sign_detection.ipynb **FASTER R-CNN**
jupyter notebook yolov8_for_sign_detection.ipynb **YOLOV8**
jupyter notebook webcam_test_signs.ipynb **TESTING YOLOV8 with webcam**

#Metrics
In this project, we use the following metrics to evaluate the performance of the models:

mAP (mean Average Precision)
Precision
Recall
Results
As a result of training the models, the following results were obtained:

YOLOv8
Mean Average Precision (mAP): 0.964
Precision for traffic signs: 0.831 for green light and 0.835 for red light.
Faster R-CNN
Mean Average Precision (mAP): 11.21
Precision for traffic signs: 11.80 for green light and 7.44 for red light.



## Installation

To install the required dependencies, run the following command:

```bash
pip install -r requirements.txt
