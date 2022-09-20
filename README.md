## _tCrop_: Thermal Imaging Based Plant Stress Identification Using On-Edge Deep Learning [[Paper](https://ieeexplore.ieee.org/abstract/document/9864547) | [Code](https://github.com/RITIK-12/tCrop)]

![vision-1](https://user-images.githubusercontent.com/54806252/188621949-0ce37341-471f-44fd-ad2f-aab3d42166b6.png)


## ✯ Abstract
Plant stress identification is one of the critical tasks to secure food availability for the future. Stress in plants increases considerably due to changing environmental conditions. This paper proposes an innovative solution for the automatic detection of plant stress using computer vision and
deep learning for edge computing platforms. The novel model classifies the disease and sends an alert to the cloud if the disease is detected for an early detection of the disease. The idea can be implemented on any edge platform, where the thermal camera captures the image of the crop, the deep learning model predicts the disease in the plant, gives the inference on edge and sends alerts if the disease is detected. The proposed novel CNN model had 90% validation accuracy and 93% test accuracy. The tCrop Lite model had 94% test accuracy and inference time of 0.001 seconds when evaluated on the Raspberry Pi 4 device.



## ✯ Datset Acquisition & Preparation
<img width="1000" alt="Screenshot 2022-09-06 at 5 35 26 PM" src="https://user-images.githubusercontent.com/54806252/188632924-79cbe23c-3b0c-486f-ab69-9bfb467d5937.png">


* Dataset having thermal images of diseased and healthy leaves of paddy crops was acquired from [1].
* It had 602 images belonging five classes namely Bacterial Leaf Blight, Blast, Leaf Spot, Hispa and Healthy leaves.
* The images were cropped to remove the temperature tags and other texts.
* Image augmentation techniques such as horizontal flip, vertical flip and rotation by 45, 90 degrees were used to remove class imbalance and  increase size of dataset.
* Images were then resized to 224x224 pixels.
* Total number of images after augmentation are 2200.
* The dataset was divided into train, validation and test dataset of 1539, 439 and 222.

<img width="1000" height="500" alt="Screenshot 2022-09-06 at 5 35 04 PM" src="https://user-images.githubusercontent.com/54806252/188633132-26bebbe5-00b8-4195-8480-801078d679fd.png">

### ✯✯ Dataset used in this research can be found [here](https://www.kaggle.com/datasets/ritikbompilwar/plantstressidentification).

## ✯ MODEL TRAINING & EVALUATION
* A novel CNN model is proposed for disease classification.
* The dense layers are used for inference along with dropout to reduce overfitting.
* Categorical Crossentropy was loss function used along with Adam optimizer and Accuracy as metrics.
* Model was trained on Google’s Collaboratory Platform  for 30 epochs.
* Model gave accuracy of 99% on training dataset and 93% on validation dataset.

<img width="1000" alt="Screenshot 2022-09-06 at 5 17 03 PM" src="https://user-images.githubusercontent.com/54806252/188632633-9248132f-3422-4a2f-9343-5615a268ebf7.png">


## ✯ Model Testing
* Model was evaluated on test dataset of 222 images.
* Owing to 94% accuracy only  14 images were misclassified.
* High precision and recall values indicate good performance of the classification model.

<img width="1000" alt="Screenshot 2022-09-06 at 5 14 54 PM" src="https://user-images.githubusercontent.com/54806252/188628543-48f98c81-0b88-4912-83a0-34304fe0ad43.png">


## ✯ BibTeX
If you find this code or paper useful, please use the following reference:

```
@INPROCEEDINGS{9864547,  
author={Bompilwar, Ritik and Singh Rathor, Surya Pratap and Das, Debanjan},  
booktitle={2022 IEEE Region 10 Symposium (TENSYMP)},   
title={tCrop: Thermal Imaging Based Plant Stress Identification Using On-Edge Deep Learning},   
year={2022},  
volume={},  
number={},  
pages={1-6},  
doi={10.1109/TENSYMP54529.2022.9864547}}
```

## ✯ References
1. https://www.kaggle.com/datasets/sujaradha/thermal-images-diseased-healthy-leaves-paddy

