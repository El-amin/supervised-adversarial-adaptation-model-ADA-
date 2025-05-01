Supervised ADA: Adversarial Discriminative Domain Adaptation in PyTorch

Adversarial Domain Adaption (ADA) addresses the challenges of domain shift in medical image classification. We showed the effectiveness of ADA in mitigating domain shift and greatly improving classification performance for diverse patient populations, contributing to the advancement of AI-driven healthcare solutions.

This repository contains an implementation of **Supervised Adversarial Discriminative Domain Adaptation (ADA)** in PyTorch. The approach enables knowledge transfer between two domains (source and target) using labeled data from both. It integrates supervised learning with adversarial domain adaptation to reduce domain shift.

## Features

- Feature extractors based on pre-trained ResNet-18 for both source and target domains.
- Shared classifier for both domains.
- Domain discriminator for adversarial training.
- Support for cross-entropy classification and domain adversarial loss.
- Tracks and plots accuracy and loss curves over training.

## Dataset

This implementation assumes two datasets:
- Source domain: Kaggle Pneumonia Dataset (e.g., Chest X-ray Images).
- Target domain: Nigerian Chest X-ray Dataset (binary: NORMAL and PNEUMONIA).

Each dataset must be organized as follows:
Dir: train/ ['COVID', 'NORMAL', 'PNEUMONIA', 'TB']
Dir: Test/ ['COVID', 'NORMAL', 'PNEUMONIA', 'TB']

### Prerequisites
- Python 3.8+
- PyTorch
- torchvision
- matplotlib
- PIL (Pillow)

Install dependencies:

#bash
pip install torch torchvision matplotlib Pillow

 Reference
This implementation is inspired by the Adversarial Discriminative Domain Adaptation (ADDA) framework, which has been extended to the supervised setting.

If you use this code, please consider citing us:
Musa, A., Prasad, R. & Hernandez, M. Addressing cross-population domain shift in chest X-ray classification through supervised adversarial domain adaptation. Sci Rep 15, 11383 (2025). https://doi.org/10.1038/s41598-025-95390-3

