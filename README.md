<h1 align="center">Denoising Fourier Noise using REDNet in Image</h1>

📘 Paper Review & Technical Response

---

## 📄 Paper Information
**Title:** Denoising Fourier Noise using REDNet in Image  
**Authors:** Thinh Duong Tan Hung, Loc Phan Minh. 
**Conference:** ICIIT 2024  
**DOI:** https://doi.org/10.1145/3654522.3654569

This repository is a **technical study and response** to the above paper.  
No source code is provided in this repository.

---

## 🎯 Purpose of This Repository
- Study and understand **Fourier Noise** in images
- Analyze the **REDNet (Residual Encoder-Decoder Network)** architecture
- Summarize experimental settings and results
- Serve as an **academic response / reading note / research portfolio**

---

## 🧠 Problem Overview
Fourier noise is a type of frequency-domain noise that significantly degrades image quality.
Traditional FFT-based denoising methods require manual threshold tuning and lack adaptability.

The paper proposes using **REDNet**, a deep learning-based residual encoder-decoder network,
to automatically learn and remove Fourier noise from images.

---

## 🏗️ Method Summary

### Fourier Noise Generation
- Images are transformed into the frequency domain
- Artificial Fourier noise is applied
- Noisy images are converted back to spatial domain

### REDNet Architecture
- Encoder–Decoder structure
- Symmetric skip connections
- Residual learning between noisy and clean images
- Input size: `(150 × 150 × 3)`
- Loss function: **Mean Squared Error (MSE)**

---

## 🧪 Experimental Setup
- Dataset: Landscape images
- Total images: 1000
- Data split:
  - Training: 72%
  - Validation: 8%
  - Testing: 20%
- Optimizer: Adam
- Learning rate: 0.0001

---

## 📊 Results (Reported in Paper)

| Metric | Value |
|------|------|
| PSNR | ~5.72 dB |
| MSE  | ~104.52 |

The results indicate that REDNet is effective in reducing Fourier noise,
although the output images remain slightly blurry.

---

## ⚠️ Limitations Discussed
- Image sharpness is not fully preserved
- Residual noise artifacts remain
- Performance limited by dataset size and model complexity

---

## 🔮 Future Directions
- Combine REDNet with super-resolution models (e.g., LapSRN)
- Apply post-processing (sharpening, filtering)
- Train with higher-resolution datasets
- Explore domain-specific Fourier noise patterns

---

## 🧑‍🎓 Author’s Note
This repository is created for:
- Academic learning
- Research understanding
- Portfolio demonstration

All credits belong to the original authors.

