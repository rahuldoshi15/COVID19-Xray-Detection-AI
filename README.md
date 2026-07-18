# COVID-19 X-ray Detection using Deep Learning

![Python](https://img.shields.io/badge/Python-3.x-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red)
![License](https://img.shields.io/badge/License-MIT-green)

## Project Overview

This project presents an automated deep learning framework for the classification of chest X-ray images using **Artificial Intelligence (AI)**. The study compares the performance of a **Custom Convolutional Neural Network (CNN)** and **MobileNetV2 (Transfer Learning)** for multiclass classification of chest X-ray images.

The system classifies chest X-ray images into four categories:

- COVID-19
- Normal
- Lung Opacity
- Viral Pneumonia

The objective is to evaluate whether transfer learning provides better classification performance than a CNN developed from scratch while maintaining computational efficiency.

---

## Project Objectives

- Develop an automated chest X-ray image classification system.
- Compare the performance of a Custom CNN and MobileNetV2.
- Evaluate the models using standard classification metrics.
- Demonstrate the effectiveness of transfer learning for medical image analysis.

---

## Dataset

This project uses the **COVID-19 Radiography Database**, publicly available on Kaggle.

**Dataset Link:**

https://www.kaggle.com/datasets/tawsifurrahman/covid19-radiography-database

The dataset contains four classes:

| Class | Images |
|--------|-------:|
| COVID-19 | 3,616 |
| Normal | 10,192 |
| Lung Opacity | 6,012 |
| Viral Pneumonia | 1,345 |
| **Total** | **21,165** |

**Note:** The dataset is **not included** in this repository because of GitHub size limitations and the dataset license.

---

## Technologies Used

- Python
- TensorFlow
- Keras
- Google Colab
- NumPy
- Pandas
- Matplotlib
- OpenCV
- Scikit-learn

---

## Project Structure

```
COVID19-Xray-Detection-AI/
│
├── dataset/                 # Dataset information
├── images/                  # Figures used in the report
├── models/                  # Trained models and histories
├── notebooks/               # Jupyter notebooks
├── processed/               # Processed CSV files and label encoder
├── report/                  # Dissertation and presentation
├── results/                 # Evaluation results
├── README.md
├── requirements.txt
└── LICENSE
```

---

## Deep Learning Models

### Model 1 – Custom CNN

- Convolution Layers
- Max Pooling
- Dropout
- Dense Layers
- Softmax Output

### Model 2 – MobileNetV2

- Transfer Learning
- ImageNet Pre-trained Weights
- Fine-tuning
- Global Average Pooling
- Softmax Classifier

---

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report

---

## Experimental Results

| Metric | Custom CNN | MobileNetV2 |
|---------|-----------:|------------:|
| Training Accuracy | 86.43% | 88.46% |
| Validation Accuracy | 78.17% | 86.83% |
| Test Accuracy | *(Refer Results Folder)* | 86.33% |

### Key Finding

The MobileNetV2 model outperformed the Custom CNN in terms of validation accuracy, generalization capability, and computational efficiency, demonstrating the effectiveness of transfer learning for chest X-ray image classification.

---

## Repository Contents

### notebooks/

Contains all notebooks used during development, including:

- Data Exploration
- Data Preprocessing
- Custom CNN
- MobileNetV2
- Model Comparison
- Model Evaluation

### models/

Contains:

- Trained Custom CNN model
- Trained MobileNetV2 model
- Training history files

### processed/

Contains processed datasets and label encoder used during model training.

### results/

Contains:

- Classification reports
- Confusion matrix
- Model comparison
- Evaluation summaries

### report/

Contains:

- Final dissertation report
- Project presentation

### images/

Contains figures used in the dissertation such as:

- System Architecture
- Workflow
- Training Accuracy
- Training Loss
- Confusion Matrix

---

## How to Run

1. Clone this repository.

```
git clone https://github.com/rahuldoshi15/COVID19-Xray-Detection-AI.git
```

2. Download the dataset from Kaggle.

3. Extract the dataset into the `dataset/` directory.

4. Install the required libraries.

```
pip install -r requirements.txt
```

5. Run the notebooks in sequence.

---

## Future Enhancements

Possible future improvements include:

- EfficientNet implementation
- DenseNet121 implementation
- ResNet50 implementation
- Vision Transformers
- Explainable AI using Grad-CAM
- Web application deployment
- Clinical validation using external datasets

---

## Academic Information

**Project Title**

**COVID-19 X-ray Detection using Deep Learning**

Submitted in partial fulfillment of the requirements for the award of the degree of

**Master of Computer Applications (MCA)**

---

## Author

**Rahul Doshi**

MCA (Artificial Intelligence)

Amrita Vishwa Vidyapeetham

---

## License

This project is licensed under the MIT License.

---

## Acknowledgement

The authors acknowledge the creators of the **COVID-19 Radiography Database** for making the dataset publicly available to support research in AI-assisted medical image analysis.
