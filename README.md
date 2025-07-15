# Enhanced Image Upscaling Using Multi-Scale Attention and Residual Block Techniques

This repository contains the code and dissertation for my Master's thesis project, which explores advanced single-image super-resolution (SISR) through the integration of Multi-Scale Attention (MSA) mechanisms and Residual Blocks within a GAN-based framework. The research targets both enhancement in image quality and interpretability of deep learning models.

## Abstract

This study proposes a novel deep learning model named EDSR-MSA, which combines the strengths of residual learning and multi-scale attention to improve the performance of image super-resolution tasks. The model is trained progressively for multiple upscaling factors (2x, 4x), and integrates Grad-CAM to provide insight into the regions of focus during resolution enhancement. The approach is evaluated using PSNR and SSIM over 100+ test samples and demonstrates both quantitative and perceptual improvements over baseline methods.

### Key Contributions

- Custom architecture combining residual learning and multi-scale attention
- Combined loss function strategy using MSE, Perceptual, and Adversarial losses
- Application of Grad-CAM for model interpretability
- Evaluation using PSNR and SSIM with additional visual analysis

## Technologies and Tools

- Programming Language: Python
- Frameworks: PyTorch, TorchVision
- Concepts: Convolutional Neural Networks, Residual Learning, GANs, Attention Mechanisms, Grad-CAM
- Libraries: numpy, scikit-image, tqdm, matplotlib, PIL, opencv-python
- Development Platform: Google Colab with NVIDIA T4 GPU
- Evaluation Metrics: PSNR, SSIM, visual inspection


## Problem Statement

Traditional super-resolution methods often fail to reconstruct fine textures or generalize well to unseen data, particularly when using interpolation-based techniques. Deep learning-based methods significantly improve image reconstruction but lack transparency. This project addresses both accuracy and interpretability using a novel architectural approach and visualization techniques.

## Interpretability with Grad-CAM

To improve model transparency, Gradient-weighted Class Activation Mapping (Grad-CAM) is applied to the final convolutional layers. This provides heatmaps indicating which parts of the input image influence the model’s predictions, helping researchers and practitioners better understand the model's behavior.

## Evaluation Results

The EDSR-MSA model was evaluated on a test set of 100 images. Performance metrics are as follows:

| Metric | Value        |
|--------|--------------|
| PSNR   | 21.4187 dB   |
| SSIM   | 0.7472       |

Visual inspections confirm improvements in sharpness and detail reconstruction, with attention maps validating the model’s focus on texture-rich and high-frequency regions.
