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

### Evaluation of the Four Models  

#### 🎭 GAN
- **Training Speed:** Fast to train per epoch.  
- **Training Stability:** Moderate; training was stable in this project but GANs are often sensitive to hyperparameters.  
- **Image Quality:** Acceptable; images were plausible but lacked fine detail.  
- **Image Diversity:** Limited; prone to repetition without major mode collapse.  
- **Computational Cost:** Low; fully connected architecture is lightweight.  

➤➤ **Summary:** A simple and fast model that can generate basic images, but struggles with detail and diversity.  

---

#### 🌀 DCGAN
- **Training Speed:** Slower than vanilla GAN due to convolutional layers.  
- **Training Stability:** Less stable; the discriminator tended to overpower the generator.  
- **Image Quality:** Improved sharpness and structure over vanilla GAN.  
- **Image Diversity:** Better than vanilla GAN.  
- **Computational Cost:** Moderate; more complex due to convolutional operations.  

➤➤ **Summary:** A more powerful GAN variant producing higher-quality images, but requiring careful balancing to ensure stable training.  

---

#### 🔀 VAE
- **Training Speed:** Fast; converges quickly and reliably.  
- **Training Stability:** Very stable due to its probabilistic framework.  
- **Image Quality:** Comparable with GANs; images are often blurrier.  
- **Image Diversity:** Good; covers more modes of the data distribution.  
- **Computational Cost:** Low to moderate.  

➤➤ **Summary:** A stable and efficient generative model with good data coverage, though image quality is usually softer.  

---

#### 🌫 Diffusion Model
- **Training Speed:** Very slow; requires many steps and long training times.  
- **Training Stability:** Very stable; training is predictable and robust.  
- **Image Quality:** High; often surpasses GANs in detail and realism.  
- **Image Diversity:** Good; captures wide variation in the data.  
- **Computational Cost:** High; both training and sampling are resource-intensive.  

➤➤ **Summary:** The most powerful model in terms of image quality and diversity, but with significant computational demands.  

---

## 📜 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.  

---

