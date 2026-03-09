# Skin Lesion Classification using Deep Learning (HAM10000)

This project implements a **Convolutional Neural Network (CNN)** in **PyTorch** to classify dermoscopy images into seven types of skin lesions using the **HAM10000 dermatology dataset**.

The goal of this project is to explore how deep learning models learn patterns from medical images while addressing challenges such as **class imbalance, dataset variability, and robust evaluation of medical AI systems**.

---

# Problem

Skin lesion datasets are often **highly imbalanced**, where common conditions dominate the dataset while rare but clinically important conditions appear much less frequently.

This project investigates how a custom CNN architecture can classify multiple dermatological conditions while handling this imbalance effectively.

---

# Dataset

**HAM10000 (Human Against Machine with 10,000 training images)**

Dataset characteristics:

- ~10,000 dermoscopy images
- 7 diagnostic categories
- Real dermatology clinic images
- Strong class imbalance

Dataset source:

https://huggingface.co/datasets/marmal88/skin_cancer

---

# Skin Conditions Classified

| Code | Condition |
|-----|-----------|
| nv | Melanocytic Nevi |
| mel | Melanoma |
| bkl | Benign Keratosis |
| bcc | Basal Cell Carcinoma |
| akiec | Actinic Keratosis |
| vasc | Vascular Lesion |
| df | Dermatofibroma |

---

# Model Architecture

The model uses a **custom CNN architecture built from scratch**.

### Architecture Overview

Input Image **(128 × 128 × 3)**

Conv Block  
Conv → BatchNorm → ReLU → Conv → BatchNorm → ReLU → MaxPool

Repeated with increasing filters:
<img width="989" height="390" alt="image" src="https://github.com/user-attachments/assets/832606b2-9bb6-4a0c-9abe-e0c9d4dbdfc8" />
<img width="1590" height="593" alt="image" src="https://github.com/user-attachments/assets/979577d7-89eb-42f3-b30f-8fdb39d4bd2d" />

