# Image Classification using CNN From Scratch and Transfer Learning

## Author

**Achmad Syahiir Marsha Wijaya**
NIM: **452024611027**
Teknik Informatika
Universitas Darussalam Gontor

---

## Project Description

This project was developed as an assignment for the Machine Learning 2 course. The objective is to compare the performance of **Convolutional Neural Network (CNN) From Scratch** and **Transfer Learning using MobileNetV2** for image classification tasks.

Two different datasets were used:

* CIFAR-10 for CNN From Scratch.
* Microsoft Cats and Dogs Dataset for Transfer Learning.

The comparison focuses on model accuracy, training efficiency, computational requirements, and practical implementation.

---

## Datasets

### 1. CIFAR-10

* 60,000 RGB images.
* 10 classes.
* 50,000 training images.
* 10,000 testing images.

Dataset Source:
https://www.tensorflow.org/datasets/catalog/cifar10

### 2. Microsoft Cats and Dogs

* Approximately 25,000 images.
* Two classes: Cat and Dog.
* Downloaded from Kaggle.

Dataset Source:
https://www.kaggle.com/datasets/shaunthesheep/microsoft-catsvsdogs-dataset

---

## Methods

### CNN From Scratch

The CNN architecture consists of:

* Convolution Layer
* Max Pooling Layer
* Flatten Layer
* Dense Layer
* Dropout Layer
* Softmax Output Layer

### Transfer Learning

The pretrained MobileNetV2 model is used with:

* MobileNetV2 Base Model
* Global Average Pooling
* Dropout Layer
* Dense Output Layer
* Fine Tuning

---

## Preprocessing

### CNN

* Load CIFAR-10 dataset.
* Normalize pixel values.
* Data augmentation.
* Batch and shuffle.

### Transfer Learning

* Extract dataset.
* Remove corrupted images.
* Resize images to 224×224.
* Data augmentation.
* MobileNetV2 preprocessing.
* Train-validation split.

---

## Experimental Results

| Model                           | Accuracy |
| ------------------------------- | -------- |
| CNN From Scratch                | 76.50%   |
| Transfer Learning (MobileNetV2) | 98.31%   |

The experimental results show that Transfer Learning outperforms CNN From Scratch in terms of accuracy and training efficiency.

---

## Technologies Used

* Python
* TensorFlow
* Keras
* Google Colab
* NumPy
* Matplotlib

---

## Project Structure

```
CNN_TL/
│
├── CNN_From_Scratch.ipynb
├── Transfer_Learning.ipynb
├── dataset/
├── images/
├── README.md
└── report.pdf
```

---

## Conclusion

CNN From Scratch successfully learned image features independently and achieved satisfactory performance. However, Transfer Learning using MobileNetV2 achieved significantly higher accuracy with shorter training time and lower computational cost.

Based on the experiments conducted, Transfer Learning is the preferred approach for image classification tasks when data and computational resources are limited.

---

## References

1. Krizhevsky, A. Learning Multiple Layers of Features from Tiny Images.
2. Sandler, M., et al. MobileNetV2: Inverted Residuals and Linear Bottlenecks.
3. Goodfellow, I., Bengio, Y., Courville. Deep Learning.
4. TensorFlow Documentation.
5. Kaggle Microsoft Cats and Dogs Dataset.

---

## Course Information

**Course:** Machine Learning 2

**University:** Universitas Darussalam Gontor

**Semester:** 2025/2026
