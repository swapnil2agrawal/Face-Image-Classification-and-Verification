
## Face Classification and Verification Using CNN

## Objective

Given an image of a person’s face, the first objective is of classifying the ID of the face. The seond objective is of determining whether two face images are of the same person and is known as face verification. This has several important applications such as deciding whether the faces from the two images are of the same person or not.

## Approach

I used Convolutional Neural Networks (CNNs) to design an end-to-end system for these tasks. 

A dataset of few thousand images of labelled ID's is used to train customized MobileNet and ResNet50 Model for the classification task. The model learned the face embeddings during classification and then transfer learning is used for the verification task. For the verification task, two images are input and the output was a score that quantifies the similarity between the faces in these images. 


## Setup

<b>Requirements</b>
    - Python 3.7
    - Jupyter Notebooks
    - AWS (to train model on cloud)
    
<b>Instructions</b>
- Download Image_classification.ipynb and open using jupyter notebook on aws with ec2 instance. 
- Train the model for 10-15 epochs and test on the dataset
- Download Image_verification.ipynb and open using jupyter notebook on aws with ec2 instance.
- Use model saved from the classification task to measure similarity between any two new image


## References

- Weiyang Liu, Yandong Wen, Zhiding Yu, Ming Li, Bhiksha Raj, and Le Song. Sphereface: Deep hypersphere embedding for face recognition. In Proceedings of the IEEE conference on computer vision and pattern recognition, pages 212–220, 2017

- Yandong Wen, Kaipeng Zhang, Zhifeng Li, and Yu Qiao. A discriminative feature learning approach for deep face recognition. In European conference on computer vision, pages 499–515. Springer, 2016.
