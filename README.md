
# 🧠 Generative Adversarial Networks (GANs) using PyTorch

Welcome to the Generative Adversarial Networks (GANs) project built using PyTorch ⚡.
This repository demonstrates how two deep neural networks — a Generator 🤖 and a Discriminator 🕵️‍♂️ — compete against each other to create realistic synthetic images.

# 🌍 Overview

The goal of this project is to train a model that can generate realistic images from random noise 🎨.

The Generator learns to create fake images that resemble real ones.

The Discriminator learns to identify whether an image is real or generated.
Through this adversarial process, the Generator gradually improves until its images are nearly indistinguishable from real data.
<img width="821" height="799" alt="Screenshot 2025-10-19 213241" src="https://github.com/user-attachments/assets/19e7846e-c54c-47de-a857-03ff4f6797a6" />

# 🧩 Architecture
🪄 Generator

Input: Random noise vector (latent space)

Process: Upsampling layers with normalization and activation functions

Output: Synthetic image resembling the dataset

| Component     | Input        | Output                | Key Layers                                      |
| ------------- | ------------ | --------------------- | ----------------------------------------------- |
| Generator     | Noise vector | Generated image       | Linear / ConvTranspose + BatchNorm + Activation |
| Discriminator | Image        | Real/Fake probability | Conv / Linear + LeakyReLU + Dropout             |


🧠 Discriminator

Input: Real or generated image

Process: Convolutional or linear layers with LeakyReLU and dropout

Output: Probability (real = 1, fake = 0)

Component	Input	Output	Key Layers
Generator	Noise vector	Generated image	Linear / ConvTranspose + BatchNorm + Activation
Discriminator	Image	Real/Fake probability	Conv / Linear + LeakyReLU + Dropout

 <img width="785" height="790" alt="Screenshot 2025-10-19 213251" src="https://github.com/user-attachments/assets/b12dfe23-f69c-4bb5-8dc1-4d6f1a5f8d19" />

# ⚙️ Requirements

🐍 Python ≥ 3.8

🔥 PyTorch

🧰 Torchvision

📊 Matplotlib

🔢 NumPy
