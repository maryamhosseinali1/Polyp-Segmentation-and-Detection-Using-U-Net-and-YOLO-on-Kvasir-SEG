# Polyp Segmentation and Detection Using U-Net and YOLO on Kvasir-SEG

## Overview
This project focuses on the detection and segmentation of polyps in gastrointestinal images, using the Kvasir-SEG dataset. U-Net was employed for image segmentation, while YOLO was used for object detection. These models were trained and evaluated to demonstrate how AI can aid in medical image analysis for colorectal cancer prevention.

### Author:
- Maryam Hosseinali

### Dataset:
The Kvasir-SEG dataset contains polyp images, masks, and bounding boxes used for training and testing the models.

## Problem Statement
Colorectal cancer is often linked to the presence of polyps in the gastrointestinal tract. Early detection through segmentation and detection of these polyps is essential for reducing the risk of cancer. This project applied artificial intelligence to automate the process.

## Models and Methodology

### 1. U-Net for Segmentation
U-Net was chosen for its ability to handle image segmentation tasks efficiently, especially in medical imaging. This model was trained to create accurate segmentation masks from the input images.

### 2. YOLO for Detection
The YOLO (You Only Look Once) algorithm was used to detect polyps by drawing bounding boxes around them in the images. YOLO is a real-time object detection model known for its speed and accuracy.

## Data Preprocessing
- Images and masks were resized to 224x224 pixels for consistency.
- Normalization was applied to scale pixel values between 0 and 1.
- Data augmentation, including image flipping and brightness adjustments, was used to improve model robustness.

## Training and Testing
- U-Net was trained using the preprocessed images and masks to segment polyps.
- YOLO was trained using bounding boxes to detect polyps.
- The dataset was split into training and testing sets to evaluate model performance on unseen data.

## Results and Analysis
- U-Net achieved **98% accuracy** in segmentation, producing masks that closely matched the real ones.
- YOLO demonstrated good performance in detecting polyps, with predicted bounding boxes aligning well with the ground truth.
- A combined visualization of segmentation masks and detection bounding boxes highlighted the complementary strengths of both models.

## Key Challenges
- Preventing overfitting was managed through data augmentation and early stopping techniques.
- Ensuring the models generalized well to new images was a significant focus during the project.

## Comparison with Benchmark
When compared to a research paper, the models developed in this project exhibited comparable, if not superior, performance in detecting and segmenting polyps.

## Future Work
Future enhancements could explore integrating U-Net and YOLO into a single pipeline to streamline the polyp detection and segmentation process.

## Conclusion
This project demonstrated the value of AI in medical image analysis, particularly for the early detection of polyps in gastrointestinal images. The experience gained from this project provides a solid foundation for future work in AI-driven healthcare solutions.


