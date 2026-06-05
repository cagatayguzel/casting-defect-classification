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

The dataset was used for supervised image classification.

---

## Models

### 1. Simple CNN
A baseline convolutional neural network trained from scratch.

### 2. ResNet18
A transfer learning-based model initialized with pretrained ImageNet weights and adapted for binary casting defect classification.

---

## Environment

The project was developed and tested in **Kaggle Notebook** using **PyTorch**.

---

## Repository Contents

- `cnn-inspection.ipynb` → main notebook containing preprocessing, training, evaluation, Grad-CAM, and demo sections
- `README.md` → project description and usage instructions

If additional figures or output images are included, they can be placed in a separate folder such as `figures/`.

---

## How to Run

1. Open the notebook in Kaggle or Jupyter.
2. Add the casting dataset to the notebook environment.
3. Run the cells for:
   - preprocessing
   - model training or model loading
   - evaluation
   - Grad-CAM visualization
   - single-image inference demo

---

## Saved Model Weights

The trained model weights are not stored directly in this repository because of GitHub file size limitations for browser uploads.

The project was developed in Kaggle Notebook, and the notebook includes the necessary code to:
- define the models
- load saved weights
- run inference on new images

For demonstration purposes, the ResNet18 model was used as the final model.

---

## Inference and Demo

The notebook includes demo cells for:

- single-image prediction
- class probability visualization
- Grad-CAM heatmap generation

These cells can be used to test the trained model on casting images and to visualize the image regions that contribute most to the prediction.

---

## Results Summary

The baseline Simple CNN successfully learned the casting defect classification task and provided strong performance.

The ResNet18 model achieved the best overall performance and clearly improved the results compared with the baseline CNN.

In addition to quantitative evaluation, Grad-CAM was used as an explainability tool to visualize the image regions influencing the model’s predictions.

---

## Notes

This repository focuses on sharing the notebook and project structure.  
The main training and inference workflow was executed in the Kaggle environment.
