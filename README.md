# Plant Disease Classification using Deep Learning

### Download the Project.ipynb file
## Overview

This project focuses on classifying plant diseases using deep learning techniques. We compare the performance of:

* A **Baseline Model**
* A **Custom Convolutional Neural Network (CNN)**
* A **ResNet50 Transfer Learning Model**

The goal is to evaluate how well different models perform on plant disease classification using image data.

---

## Dataset

We use the **PlantVillage dataset**.

🔗 Download from Kaggle:
https://www.kaggle.com/datasets/emmarex/plantdisease

### Dataset Setup

After downloading:

1. Extract the dataset
2. Place it inside your project folder as:

```bash
dataset/
   ├── class1/
   ├── class2/
   ├── class3/
   └── ...
```

---

## Requirements

Install the required libraries:

```bash
pip install tensorflow matplotlib numpy
```

---

## How to Run the Project

1. Clone this repository:

```bash
git clone <your-repo-link>
cd <your-repo-name>
```

2. Make sure dataset is placed correctly (see above)

3. Open Jupyter Notebook:

```bash
jupyter notebook
```

4. Open the `.ipynb` file and click:
   **Run → Run All Cells**

---

## Models Implemented

### Baseline Model

* Simple neural network
* Used as a reference for comparison

### Custom CNN Model

* 3 Convolution layers
* MaxPooling layers
* Dense layers
* Learns domain-specific features

### ResNet50 (Transfer Learning)

* Pre-trained on ImageNet
* Frozen base layers
* Fine-tuned top layers

---

## Training Details

* Optimizer: Adam
* Loss Function: Categorical Crossentropy
* Batch Size: 32
* Epochs: 5

---

## Results

| Model      | Test Accuracy |
| ---------- | ------------- |
| Custom CNN | **93.25%**    |
| ResNet50   | 67.27%        |

he custom CNN significantly outperforms ResNet50 due to better domain-specific feature learning.

---

## Evaluation & Visualization

The notebook includes:

* Accuracy plots (training vs validation)
* Confusion matrices
* Sample predictions (error analysis)

---

## Key Observations

* Custom CNN performs better than transfer learning in this domain
* ResNet50 struggles due to domain mismatch
* Data augmentation improves generalization

---

## Important Notes

* Make sure dataset path is correct
* Run all cells before viewing results
* Outputs must be visible in the notebook (important for grading)

---

## Authors

* Sai Charan Nutheti
* Bala Nikhil Pasala
* Muni Sai Chetan Reddy Peddesugari

---


---
