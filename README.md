# Generative-Adversarial-Network-GANS-Using-Pytorch

🧠 Generative Adversarial Networks (GANs) using PyTorch

Welcome to the Generative Adversarial Networks (GANs) project built using PyTorch ⚡.
This repository demonstrates how two deep neural networks — a Generator 🤖 and a Discriminator 🕵️‍♂️ — compete against each other to create realistic synthetic images.

🌍 Overview

The goal of this project is to train a model that can generate realistic images from random noise 🎨.

The Generator learns to create fake images that resemble real ones.

The Discriminator learns to identify whether an image is real or generated.
Through this adversarial process, the Generator gradually improves until its images are nearly indistinguishable from real data.

🧩 Architecture
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
