# 🧬 Deep Learning-Based Cervical Cell Classification Using Pap Smear Images

### 🔬 Pap Smear Image Classification using MobileNetV2 & Transfer Learning

A deep learning-based medical image classification project that classifies **Pap smear cervical cell images** into three categories: **Normal, Moderate Dysplastic, and Severe Dysplastic**.

This project was developed as part of a **6-week Summer Internship** under the guidance of **Dr. Suman Nelaturi**.

---

## 📌 About the Project

Cervical cell classification from Pap smear images is an important computer vision problem in medical image analysis. Manual examination of cytology images requires careful observation of cellular morphology and can be time-consuming.

The objective of this project is to develop a **deep learning-based image classification system** that can learn visual features from cervical cell images and classify them into different cell categories.

A **MobileNetV2 pretrained model** is used as the backbone, and **Transfer Learning** is applied to adapt the pretrained network to the cervical cell classification task.

The complete workflow includes:

📂 Dataset Preparation  
⚖️ Dataset Balancing  
🖼️ Image Preprocessing  
🔄 Data Augmentation  
🧠 Transfer Learning  
🏋️ Model Training  
📊 Model Evaluation  
🔍 Individual Image Prediction  

---

## 🎯 Project Objectives

The main objectives of this project are:

- 🧬 Develop a deep learning model for cervical cell image classification
- 📂 Prepare and organize Pap smear image data
- ⚖️ Create a balanced dataset across the three classes
- 🖼️ Preprocess images for deep learning
- 🔄 Apply image augmentation techniques
- 🧠 Implement MobileNetV2 using Transfer Learning
- 🏋️ Train the model using TensorFlow and Keras
- 📊 Evaluate classification performance using multiple metrics
- 🔍 Test the trained model on individual cervical cell images

---

## 🗂️ Dataset

The project uses a **Cervical Cell Image Database** containing Pap smear cervical cell images.

The original dataset contains different types of cervical cells. For this project, the normal cell categories were combined to form a single **Normal** class.

The final dataset was balanced so that each target class contains an equal number of images.

### 📊 Final Dataset Distribution

| 🧬 Class | 🖼️ Number of Images |
|---|---:|
| 🟢 Normal | 292 |
| 🟡 Moderate Dysplastic | 292 |
| 🔴 Severe Dysplastic | 292 |
| **📦 Total** | **876** |

### 📌 Dataset Classes

#### 🟢 Normal
Images representing normal cervical cells.

#### 🟡 Moderate Dysplastic
Images representing moderately dysplastic cervical cells.

#### 🔴 Severe Dysplastic
Images representing severely dysplastic cervical cells.

---

## ✂️ Dataset Split

The balanced dataset was divided into training, validation, and testing sets.

| Dataset | Percentage | Images |
|---|---:|---:|
| 🏋️ Training | 70% | 612 |
| 🔎 Validation | 15% | 132 |
| 🧪 Testing | 15% | 132 |
| **📦 Total** | **100%** | **876** |

The test set was kept separate from the training process and was used for the final evaluation of the trained model.

---

# 🖼️ Image Preprocessing

Before feeding the images into the neural network, preprocessing was performed to make them suitable for the MobileNetV2 architecture.

### 🔧 Preprocessing Steps

**1. 📐 Image Resizing**

All images were resized to:

```text
224 × 224 pixels
