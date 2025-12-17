<h1 align="center">Denoising Fourier Noise using REDNet in Image</h1>

## 📄 Paper Reference
This repository is a simple implementation and reproduction of the paper:

**Denoising Fourier Noise using REDNet in Image**  
Thinh Duong Tan Hung et al., ICIIT 2024  
https://doi.org/10.1145/3654522.3654569 :contentReference[oaicite:0]{index=0}

---

## 🎯 Objective
The goal of this project is to reproduce and understand the effectiveness of  
**Residual Encoder-Decoder Network (REDNet)** for removing **Fourier (frequency-domain) noise** from images.

This repository is created as:
- A learning-based response to the original paper
- A simple academic reproduction
- A reference implementation for image denoising tasks

---

## 🧠 Method Overview
- Apply **Fourier Noise** to clean images
- Train a **REDNet (Residual Encoder-Decoder Network)** model
- Use **skip connections** to preserve spatial and frequency information
- Optimize using **MSE loss** and **Adam optimizer**

**Input size:** `(150, 150, 3)`  
**Loss function:** Mean Squared Error (MSE)

---

## 🏗️ Model Architecture
- Encoder: 5 Conv2D layers
- Decoder: 5 Conv2DTranspose layers
- Skip connections between encoder and decoder layers
- Residual learning strategy

The architecture follows the REDNet design proposed in the paper.

---

## 🚀 How to Run

### 1️⃣ Install dependencies
```bash
pip install -r requirements.txt
