# Lab 3: Padding, Strides and Object Detection using R-CNN

## Lab Overview

This lab focuses on understanding fundamental convolution operations and applying them to advanced computer vision tasks. Two practicals are covered: Padding & Strides in Convolutional Neural Networks and Object Detection using the R-CNN algorithm. The first practical builds a strong foundation in how CNNs process images, while the second demonstrates object detection using region-based deep learning techniques.

---

# Practical 1: Understanding Padding and Strides in CNN

## Practical Overview

This practical demonstrates how padding and strides affect the output of convolutional layers in a Convolutional Neural Network (CNN). The objective is to understand how feature maps are generated and how spatial dimensions change during convolution operations.

---

## Key Concepts / Techniques

- Convolution Operation  
- Padding (Valid & Same)  
- Stride  
- Feature Maps  
- Kernel / Filter  
- Output Size Calculation  
- CNN Fundamentals  

---

## How It Works

1. An input image is passed through a convolutional layer.  
2. A kernel (filter) slides over the image.  
3. Stride determines how many pixels the filter moves at each step.  
4. Padding is applied to control output size.  
5. Feature maps are generated after applying convolution.  
6. Output dimensions are calculated based on input size, kernel size, padding, and stride.  

---

## Results

The practical demonstrates how different padding and stride values impact the output feature map size. It helps in understanding how spatial information is preserved or reduced in CNN architectures.

---

## Use Case

- Designing CNN architectures  
- Image classification models  
- Feature extraction in deep learning  
- Optimizing model performance  

---

## Conclusion

This practical provides a fundamental understanding of how convolution works in neural networks. Padding and strides play a crucial role in controlling output dimensions and preserving important image features.

---

# Practical 2: Object Detection using R-CNN

## Practical Overview

This practical demonstrates the implementation of the R-CNN (Region-based Convolutional Neural Network) algorithm for object detection. The objective is to identify and localize objects within an image by generating region proposals and classifying them.

---

## Key Concepts / Techniques

- Object Detection  
- Region-based CNN (R-CNN)  
- Selective Search  
- Bounding Boxes  
- Feature Extraction using CNN  
- Image Classification  
- Deep Learning  

---

## How It Works

1. Input image is provided to the system.  
2. Selective Search algorithm generates region proposals.  
3. Each region is resized and passed through a CNN.  
4. Features are extracted for each region.  
5. A classifier predicts the object class.  
6. Bounding boxes are drawn around detected objects.  

---

## Results

The R-CNN model successfully detects and localizes objects in images. It demonstrates how deep learning can be used for both classification and localization tasks.

---

## Use Case

- Autonomous vehicles (object detection)  
- Surveillance systems  
- Face detection systems  
- Retail product detection  
- Medical object detection  

---

## Conclusion

This practical highlights the application of deep learning in object detection. R-CNN is a foundational approach that paved the way for faster and more efficient models like Fast R-CNN and YOLO.
