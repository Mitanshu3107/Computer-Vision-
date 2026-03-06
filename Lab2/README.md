# Lab 2: Semantic Segmentation and Object Detection

## Lab Overview

This lab focuses on advanced computer vision techniques used for scene understanding and object detection. The first practical explores semantic segmentation using the U-Net architecture, which performs pixel-level classification to generate segmentation masks from input images. The second practical implements real-time object detection using the YOLOv8 algorithm to identify and localize objects in live video or webcam streams. Together, these practicals demonstrate two fundamental approaches in modern computer vision: dense prediction through segmentation and object localization through detection.

---

# Semantic Segmentation using U-Net

## Practical Overview

This practical demonstrates semantic segmentation using the U-Net deep learning architecture. The objective is to train a model capable of performing pixel-level classification to distinguish foreground objects from the background. The U-Net model processes an input image and generates a corresponding binary mask where each pixel is classified according to its semantic category. This approach is widely used in applications where precise object boundaries are required.

---

## Key Concepts / Techniques

- Semantic Segmentation  
- U-Net Architecture  
- Encoder–Decoder Networks  
- Pixel-level Classification  
- Binary Mask Generation  
- Convolutional Neural Networks (CNN)  
- TensorFlow and Keras Deep Learning Framework

---

## How It Works

1. A dataset containing images and corresponding segmentation masks is prepared for training.  
2. Input images are preprocessed and resized to a uniform dimension.  
3. A U-Net model is constructed using an encoder–decoder architecture with skip connections.  
4. The encoder extracts hierarchical features while the decoder reconstructs spatial details for segmentation.  
5. The model is trained using labeled images and masks to learn pixel-level classifications.  
6. After training, the model predicts segmentation masks for new input images.  
7. Predicted masks are visualized alongside original images to evaluate segmentation performance.

---

## Results

The trained U-Net model successfully generates binary segmentation masks that separate the target object from the background. The model learns spatial and contextual features from training data, allowing accurate identification of object boundaries within images.

---

## Use Case

Semantic segmentation is widely used in industrial and real-world computer vision systems, including:

- **Medical Image Analysis** – Segmenting tumors, organs, and anatomical structures.  
- **Autonomous Driving Systems** – Identifying roads, pedestrians, vehicles, and traffic signs.  
- **Satellite and Remote Sensing** – Land cover classification and environmental monitoring.  
- **Industrial Inspection Systems** – Detecting defects and anomalies in manufactured components.  
- **Agricultural Monitoring** – Identifying crop regions and plant diseases.

---

## Conclusion

This practical demonstrates the use of the U-Net architecture for semantic segmentation tasks. By performing pixel-level classification, the model provides detailed understanding of image content. Such segmentation techniques are essential in applications where precise spatial information is required.

---

# Object Detection with YOLO

## Practical Overview

This practical demonstrates real-time object detection using the YOLOv8 (You Only Look Once) algorithm. YOLOv8 is a deep learning–based detection framework capable of identifying multiple objects in images or video streams while providing bounding boxes and class labels. The system processes live webcam or video input to detect and localize objects in real time.

---

## Key Concepts / Techniques

- Object Detection  
- YOLOv8 Architecture  
- Real-time Detection Systems  
- Bounding Box Prediction  
- Deep Learning-based Vision Models  
- Ultralytics YOLO Framework  
- Video Stream Processing

---

## How It Works

1. The YOLOv8 model is loaded using the Ultralytics framework.  
2. A webcam or video stream is initialized to capture real-time frames.  
3. Each frame is passed through the YOLOv8 model for inference.  
4. The model detects objects and predicts bounding boxes along with class labels and confidence scores.  
5. Detected objects are highlighted on the frame using bounding boxes.  
6. The processed video stream is displayed with real-time detection results.

---

## Results

The YOLOv8 model successfully detects and localizes multiple objects in real time from a webcam or video stream. The system demonstrates high detection speed while maintaining strong accuracy, enabling real-time object recognition.

---

## Use Case

YOLO-based object detection systems are widely deployed in industrial and real-world applications, including:

- **Smart Surveillance Systems** – Detecting people, vehicles, and suspicious activities.  
- **Autonomous Vehicles** – Identifying obstacles, pedestrians, and traffic signs.  
- **Retail Analytics** – Monitoring customer behavior and product interactions.  
- **Industrial Safety Monitoring** – Detecting workers and safety equipment in hazardous environments.  
- **Robotics and Automation** – Enabling robots to recognize and interact with objects.

---

## Conclusion

This practical demonstrates the implementation of the YOLOv8 algorithm for real-time object detection. By combining deep learning with efficient detection architecture, YOLO enables fast and accurate recognition of objects in dynamic environments. Understanding such detection systems is essential for building modern computer vision applications.
