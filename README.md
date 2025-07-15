# Enhanced Image Upscaling Using Multi-Scale Attention and Residual Block Techniques

This repository contains the Master's thesis and supporting materials for a novel image super-resolution model combining **Multi-Scale Attention (MSA)** mechanisms and **Residual Blocks**.

📄 **[View the full dissertation](./thesis.pdf)**

---

## 🧠 Abstract

This project explores the integration of **multi-scale attention mechanisms** and **residual blocks** within a deep learning architecture for single-image super-resolution (SR). The proposed **EDSR-MSA model** employs a progressive GAN-based framework trained at 2x and 4x scales. It also incorporates **Grad-CAM** for interpretability, helping visualize attention regions during upscaling.

**Key Contributions:**
- Novel architecture combining residual learning with multi-scale attention.
- Training strategy using MSE, perceptual, and adversarial losses.
- Use of **Grad-CAM** to visualize attention maps.
- Evaluated using PSNR and SSIM over 100 test images.

---

## 🧪 Technologies Used

- Python
- PyTorch
- Google Colab with NVIDIA T4 GPU
- Libraries: `torch`, `torchvision`, `skimage`, `numpy`, `tqdm`

---

## 📊 Results

| Metric      | Value     |
|-------------|-----------|
| PSNR        | 21.4187 dB |
| SSIM        | 0.7472    |

The model demonstrates competitive performance, with visual improvements and deeper interpretability via Grad-CAM.

---

## 🖼️ Sample Results

> Include before/after sample image comparisons in the `results/` folder if available.

---

## 🔍 Interpretability with Grad-CAM

Grad-CAM was applied to visualize areas of the image the model focuses on during upscaling. This helped interpret and validate the model’s decision-making process.

---

## 📁 Project Structure
