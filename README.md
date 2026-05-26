# ConvNeXtV2 Intel Scene Classification

Scene classification project using ConvNeXtV2 and transfer learning in PyTorch on the Intel Image Classification dataset.

## Overview

This project focuses on natural scene image classification using a modern ConvNeXtV2 backbone with transfer learning techniques. The model was trained and fine-tuned using PyTorch with mixed precision training, checkpoint saving, reproducibility settings, and validation-based model selection.

The project achieved strong validation performance and was also tested on external real-world images from Unsplash and web sources.

## Notebook Links

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1_k8wSGIv3wtyRfYmjVdS8n_IQ2dpy-z9?usp=sharing)

[![View In Kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/code/mihirvyas/cnnintelclassification)

---

## Dataset Link

[![Dataset](https://img.shields.io/badge/Dataset-Intel%20Image%20Classification-blue)](https://www.kaggle.com/datasets/puneet6060/intel-image-classification)

---

## Dataset

Dataset Used:
- Intel Image Classification Dataset

Classes:
- Buildings
- Forest
- Glacier
- Mountain
- Sea
- Street

---

## Model Architecture

Backbone:
- ConvNeXtV2 Tiny (`convnextv2_tiny.fcmae_ft_in22k_in1k`)

Classifier Head:
- Linear Layer (128 hidden units)
- ReLU Activation
- Output Layer (6 classes)

---

## Training Features

- Transfer Learning
- Partial Fine-Tuning
- Mixed Precision Training (AMP)
- Validation Checkpoint Saving
- Reproducible Training Seed
- GPU Training
- Custom Classification Head
- Early Best-Model Saving Logic

---

## Performance

Best Validation Accuracy:
- **95.1%**

Validation Loss:
- ~0.155

The best model checkpoint is automatically saved based on validation accuracy.

---

## Inference Testing

The trained model was tested on:
- Dataset validation images
- External Unsplash/web images

The model generalized well on unseen natural scene images.

---

## Technologies Used

- Python
- PyTorch
- timm
- Torchvision
- NumPy
- PIL
- Kaggle Notebook Environment

---

## Project Structure

```bash
.
├── notebook.ipynb
├── best_model.pth
└── README.md
