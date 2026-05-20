# ConvNeXtV2 Intel Scene Classification

Scene classification project using ConvNeXtV2 and transfer learning in PyTorch on the Intel Image Classification dataset.

## Overview

This project focuses on natural scene image classification using a modern ConvNeXtV2 backbone with transfer learning techniques. The model was trained and fine-tuned using PyTorch with mixed precision training, checkpoint saving, reproducibility settings, and validation-based model selection.

The project achieved strong validation performance and was also tested on external real-world images from Unsplash and web sources.

## Notebook Links

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]([https://YOUR_COLAB_LINK_HERE](https://colab.research.google.com/#fileId=https%3A//storage.googleapis.com/kaggle-colab-exported-notebooks/mihirvyas/cnnintelclassification.6d007670-ba0d-4926-aa1f-6aa08d841c26.ipynb%3FX-Goog-Algorithm%3DGOOG4-RSA-SHA256%26X-Goog-Credential%3Dgcp-kaggle-com%2540kaggle-161607.iam.gserviceaccount.com/20260520/auto/storage/goog4_request%26X-Goog-Date%3D20260520T125827Z%26X-Goog-Expires%3D259200%26X-Goog-SignedHeaders%3Dhost%26X-Goog-Signature%3D99eb47f312fbbef3fd72f23b89fd73d77b156e565109bff50ef5b3b1cbecc9e9e46fb7e8c2bfae72ecb04fdd8f604c6678af685d937e70fe98a7ae15227d5887e12436e0e4e399350594d73f007945b3d676afb1ba24ad362d172e3a36ba8f9e4e027c12c35d251a43d1cb9c29b4a6274fc0158fe65b8c3c23042985067a5afac3797cd8199ae028739a34b0153ef2fa69b9acc96d65779aaee6796d61c23365071fd7ff700c78033c529cfeac4a605ca335f66724c96266796fcd24cec0111dba3541b1653b179e33d82a4ff92f7eaee08caca58359eaecaa9a0f8afccf28e5e1769f5284826a2eac4b0188c9e353e92a8a9762131da56db95a88207030c4a1))

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
