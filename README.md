# Anime Face Generation using DCGAN

## Project Overview
This project implements a **Deep Convolutional Generative Adversarial Network (DCGAN)** to generate anime-style face images from random noise.

## Dataset
- **Name:** Anime Faces
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/soumikrakshit/anime-faces)
- **Total Images:** 43,102
- **Resolution:** 64×64

## Model Details
| Component       | Details                                     |
|----------------|----------------------------------------------|
| Generator      | ConvTranspose2d + BatchNorm + ReLU + Tanh    |
| Discriminator  | Conv2d + LeakyReLU + BatchNorm + Sigmoid     |
| Latent Size    | 100                                          |
| Optimizer      | Adam (lr=0.0002, β1=0.5, β2=0.999)           |
| Loss Function  | Binary Cross Entropy (BCE)                   |
| Epochs         | 25                                           |
| GPU            | Tesla T4                                     |

## Results
Sample generated faces are available in `final_anime_faces.png`.

## How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
