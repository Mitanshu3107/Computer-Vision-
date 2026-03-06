# Lab 1: Image Classification using CNN and Transfer Learning

## Lab Overview

This lab focuses on implementing image classification techniques using deep learning. Two approaches are explored: training a Convolutional Neural Network (CNN) from scratch and applying transfer learning using a pre-trained deep neural network. The first practical demonstrates fundamental CNN-based classification on the CIFAR-10 dataset, while the second practical applies transfer learning using the VGG16 architecture for binary classification on the Cats vs Dogs dataset.

---

# Practical 1: Implementing Basic Image Classification on CIFAR-10 with CNNs

## Practical Overview

This practical demonstrates the implementation of a Convolutional Neural Network (CNN) for multi-class image classification using the CIFAR-10 dataset. The objective is to build and train a CNN model from scratch to learn hierarchical visual features directly from raw image data and classify images into ten object categories.

---

## Key Concepts / Techniques

- Convolutional Neural Networks (CNN)
- Image Classification
- CIFAR-10 Dataset
- Convolution and Pooling Layers
- Batch Normalization
- Dropout Regularization
- TensorFlow / Keras Deep Learning Framework

---

## How It Works

1. The CIFAR-10 dataset is loaded and split into training and testing sets.
2. Image pixel values are normalized to improve model convergence.
3. A CNN architecture is constructed using convolutional, pooling, batch normalization, and dropout layers.
4. The network learns hierarchical visual features from the dataset during training.
5. The trained model is evaluated using test accuracy and performance metrics.
6. Predictions are visualized to verify classification performance.

---

## Results

The CNN model successfully learns visual patterns from the CIFAR-10 dataset and classifies images into ten categories such as airplanes, automobiles, birds, cats, and dogs. The training and validation curves demonstrate how the model improves over multiple training epochs while learning discriminative image features.

---

## Use Case

CNN-based image classification systems are widely applied in industrial and real-world scenarios such as:

- Automated quality inspection in manufacturing
- Traffic sign recognition in autonomous vehicles
- Retail product recognition systems
- Medical image classification
- Satellite and remote sensing image analysis

---

## Conclusion

This practical demonstrates how Convolutional Neural Networks can automatically learn hierarchical image features for classification tasks. Training a CNN from scratch provides a fundamental understanding of deep learning-based image recognition systems.

---

# Practical 2: Transfer Learning with VGG16 for Cats vs Dogs Classification

## Practical Overview

This practical demonstrates the use of transfer learning for image classification using the pre-trained VGG16 convolutional neural network. Instead of training a deep network from scratch, the model leverages feature representations learned from the large-scale ImageNet dataset and adapts them to perform binary classification on the Cats vs Dogs dataset.

---

## Key Concepts / Techniques

- Transfer Learning
- Pre-trained Convolutional Neural Networks
- VGG16 Architecture
- Fine-tuning Deep Neural Networks
- Image Data Augmentation
- Binary Image Classification
- Feature Extraction using CNNs
- TensorFlow / Keras Implementation

---

## How It Works

1. The Cats vs Dogs dataset is organized into training and validation directories.
2. Image data augmentation is applied to improve model generalization.
3. The pre-trained VGG16 model is loaded with ImageNet weights while excluding its original classification layers.
4. The convolutional base of VGG16 is initially frozen to preserve learned features.
5. Custom fully connected layers are added for binary classification.
6. The model is trained to distinguish between cats and dogs.
7. Selected layers of VGG16 are later unfrozen and fine-tuned with a lower learning rate.

---

## Results

The transfer learning approach achieves strong classification performance with high validation accuracy. By leveraging pre-trained feature representations from VGG16, the model effectively distinguishes between cats and dogs with reduced training time and improved generalization.

---

## Use Case

Transfer learning-based image classification systems are widely used in industrial computer vision applications, including:

- Automated product recognition in retail and e-commerce
- Medical image classification and diagnostic assistance
- Wildlife monitoring and species identification
- Smart surveillance and object recognition systems
- Visual content moderation platforms

---

## Conclusion

This practical highlights the advantages of transfer learning in modern computer vision tasks. By adapting a pre-trained VGG16 network, high classification accuracy can be achieved with limited data and reduced computational cost. Transfer learning is widely used in industrial AI systems where labeled datasets may be limited.
