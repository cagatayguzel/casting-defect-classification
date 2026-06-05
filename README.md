# Automated Visual Inspection of Casting Products Using Deep Learning

This project investigates deep learning-based casting defect classification using image data. The task is formulated as a binary image classification problem in which casting product images are classified as **defective** or **non-defective**.

Two different models were evaluated:

- **Simple CNN** as a baseline model
- **ResNet18** as a transfer learning-based model

The final results showed that ResNet18 outperformed the baseline CNN and was selected as the final model.

---

## Dataset

The experiments were conducted using a public Kaggle casting product dataset with two classes:

- `def_front` → defective  
- `ok_front` → non-defective  

The dataset is accessed directly from Kaggle within the notebook environment.

---

## Models

### 1. Simple CNN
A baseline convolutional neural network.

### 2. ResNet18
A transfer learning-based model initialized with pretrained ImageNet weights and adapted for binary casting defect classification.

---

## Environment

The project was developed and tested in **Kaggle Notebook** using **PyTorch**.

To properly run the code and access the dataset, it is recommended to execute the notebook directly in Kaggle.

📌 Kaggle Notebook Link: *(https://www.kaggle.com/code/cagatayguzel/cnn-inspection)*

---

## Repository Contents

- `cnn-inspection.ipynb` → main notebook containing preprocessing, model loading, evaluation, Grad-CAM, and demo sections  
- `README.md` → project description and usage instructions  

---

## How to Run

1. Open the notebook in Kaggle using the link above.
2. Run all cells in order.

The notebook is configured to **skip training** and **automatically load pretrained model weights**, allowing direct evaluation and inference without retraining.

---

## Saved Model Weights

Due to GitHub file size limitations, trained model weights are not stored in this repository.

Instead, the notebook is designed to load pretrained weights directly from the Kaggle environment.

---

## Inference and Demo

The notebook includes demo sections for:

- single-image prediction  
- class probability visualization  
- Grad-CAM heatmap generation  

These can be used to test the trained model and visualize the regions that contribute most to the prediction.

---

## Results Summary

Both models successfully learned the casting defect classification task.

The ResNet18 model achieved the best overall performance and showed clear improvements over the baseline CNN.

Grad-CAM was used as an explainability tool to visualize the image regions influencing the model’s predictions.

---

## Notes

- The notebook is configured for **inference-only execution** (training is disabled).
- All experiments and model execution are intended to run within the Kaggle environment.
- Running the notebook locally may require manual dataset and weight configuration.
