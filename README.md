# Sentiment Analysis on Amazon Reviews with Apache Spark and Spark NLP
## Overview
This project delves into the ethical dimensions of generative AI art, particularly focusing on the potential ramifications of synthetic images in various societal contexts. It explores the ongoing debate surrounding the validity of such art forms and raises critical ethical considerations regarding their use in formal settings like politics, business, and decision-making processes.

To tackle the task of image classification, five different convolutional neural network (CNN) architectures are employed. CNNs are well-suited for discerning patterns and features crucial for categorizing images accurately. Each model is meticulously tuned to optimize its classification performance, with the overarching objective of identifying the model that yields the highest test accuracy.

## Dataset 
The investigation utilizes the CIFAR-10 dataset, comprising 60,000 32x32 colored images across ten distinct categories. These categories encompass objects ranging from airplanes to trucks, with a clear demarcation between real and synthetic images. The training dataset consists of 80,000 labeled images equally distributed between real and fake categories, while both the validation and test sets comprise 20,000 labeled images each, evenly split between the two classes. The data source could be found here: https://www.kaggle.com/datasets/birdy654/cifake-real-and-ai-generated-synthetic-images

## CNN Models
We deployed five distinct architectures to perform image classification:

- ConvNeXt
- AlexNet
- ResNet50
- LeNet5
- EfficientNetV2

The GitHub repository contains code for all five modeling approaches.

## Objectives
- Compare and evaluate performance of all five CNN models.
- Assess classfication accuracy of fake and real images by applying these five models.

## Results
- Models were evaluated based on accuracy with differenct choices of hyperparameters.
- Support Vector Machine performed the best, achieving high accuracy across all metrics.
  
## Conclusion
- Fine-tuning hyperparameters such as learning rate, batch size, and epochs could significantly enhance the model's ability to differentiate between real and fake images, thereby increasing accuracy and precision.
- Extending the training duration and increasing the number of epochs in future experiments may lead to decreased loss and improved accuracy as the model learns from data over a longer period, enabling it to capture more subtle features that distinguish real from fake images.
- Transitioning from the CIFAR dataset, which consists of tiny, low-resolution images, to real-world datasets containing more varied and high-resolution images would provide a more realistic testing environment and enhance the model's applicability in practical settings, such as content verification.
