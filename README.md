# 👗 Fashion MNIST Generative Models

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)  
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)](https://www.tensorflow.org/)  
[![Google Colab](https://img.shields.io/badge/Platform-Google%20Colab-green)](https://colab.research.google.com/)

---

## 📌 Project Summary

This project focuses on **generating Fashion MNIST images** using four state-of-the-art deep learning models:  

- 🎭 **Generative Adversarial Network (GAN)**  
- 🌀 **Deep Convolutional GAN (DCGAN)**  
- 🔀 **Variational Autoencoder (VAE)**  
- 🌫 **Denoising Diffusion Probabilistic Model (DDPM)**  

The models were evaluated based on the **visual quality** and **diversity** of the synthesized fashion images.

---

## ⚙️ Tools & Environment

- **Language:** Python  
- **Framework:** [TensorFlow 2](https://www.tensorflow.org/)  
- **Platform:** Google Colab (with GPU acceleration)  

---

## 🧵 Dataset

The project uses the **Fashion MNIST** dataset, consisting of:  
- 28×28 grayscale images  
- 10 clothing categories (e.g., T-shirts, trousers, shoes, coats, bags, etc.)  
- Balanced between complexity and simplicity  
- Preprocessing: **Normalization & scaling** to fit model inputs  

---

## 🧠 Model Architectures

### 1. 🎭 Generative Adversarial Network (GAN)
- **Structure:** Dense layers (fully connected)  
- **Training:** Stable, no mode collapse  
- **Result:** Generated plausible images, though not the sharpest  

---

### 2. 🌀 Deep Convolutional GAN (DCGAN)
- **Structure:** Convolutional & transposed convolutional layers  
- **Stabilization:** Batch Normalization + LeakyReLU  
- **Challenge:** Discriminator overpowering generator  
- **Solution:** Periodic weight reversion for discriminator  
- **Result:** Sharper and more structured images  

---

### 3. 🔀 Variational Autoencoder (VAE)
- **Structure:** Probabilistic encoder-decoder framework  
- **Latent Space:** Well-structured, meaningful feature representation  
- **Result:** Blurrier images but stable & fast training  

---

### 4. 🌫 Denoising Diffusion Probabilistic Model (DDPM)
- **Process:** Gradually adds noise and learns to denoise  
- **Cost:** Longer training & inference times  
- **Result:** **Highest quality** and **most detailed** fashion images  

---

## 🎨 Results & Observations

- **GAN:** Basic but stable, moderate image quality  
- **DCGAN:** Better structure & sharpness, needed balancing tricks  
- **VAE:** Blurrier but stable & interpretable latent space  
- **Diffusion Model:** Best results, but computationally expensive  

> Each model demonstrates trade-offs between **training stability**, **image quality/diversity**, and **computational cost**.

---

## 📜 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.  

---
