## _tCrop_: Thermal Imaging Based Plant Stress Identification Using On-Edge Deep Learning [[Paper](https://ieeexplore.ieee.org/abstract/document/9864547) | [Code](https://github.com/RITIK-12/tCrop)]

![vision-1](https://user-images.githubusercontent.com/54806252/188621949-0ce37341-471f-44fd-ad2f-aab3d42166b6.png)


## Abstract
Plant stress identification is one of the critical tasks to secure food availability for the future. Stress in plants increases considerably due to changing environmental conditions. This paper proposes an innovative solution for the automatic detection of plant stress using computer vision and
deep learning for edge computing platforms. The novel model classifies the disease and sends an alert to the cloud if the disease is detected for an early detection of the disease. The idea can be implemented on any edge platform, where the thermal camera captures the image of the crop, the deep learning model predicts the disease in the plant, gives the inference on edge and sends alerts if the disease is detected. The proposed novel CNN model had 90% validation accuracy and 93% test accuracy. The tCrop Lite model had 94% test accuracy and inference time of 0.001 seconds when evaluated on the Raspberry Pi 4 device.



## Datset Acquisition & Preparation
![augmentation-1](https://user-images.githubusercontent.com/54806252/188620280-173af13c-ad0a-4297-b652-7803dab7a1d1.png)
i. The images were cropped to remove the temperature tags and other texts.
ii. Image augmentation techniques such as horizontal flip, vertical flip and rotation by 45, 90 degrees were used to remove class imbalance and  increase size of dataset.
iii. Images were then resized to 224x224 pixels.
iv. Total number of images after augmentation are 2200.
v. The dataset was divided into train, validation and test dataset of 1539, 439 and 222.


## BibTeX
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
