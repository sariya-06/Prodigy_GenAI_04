🏗 Pix2Pix – Image-to-Image Translation using Conditional GAN
📌 Project Overview

This project implements Pix2Pix (Conditional GAN) for image-to-image translation.
The model learns to translate a building photo into its corresponding semantic segmentation map.

The architecture consists of:

Generator → U-Net architecture

Discriminator → PatchGAN

Loss Function → Adversarial Loss + L1 Loss

🧠 Model Architecture
🔹 Generator (U-Net)

Encoder-Decoder structure

Skip connections for better feature transfer

Captures both low-level and high-level features

🔹 Discriminator (PatchGAN)

Classifies image patches instead of full image

Helps generate sharper and realistic outputs

📂 Dataset

Used a paired dataset (Input | Target format)

Each training image contains:

Left side → Input Image

Right side → Target Image

Example:
Building Photo ➝ Segmentation Map

⚙ Training Details

Epochs: 50+

Optimizer: Adam

Batch Size: 1

Image Size: 256×256

Framework: TensorFlow

📊 Results

The model successfully generates segmentation maps that closely resemble ground truth images.

Comparison includes:

Input Image

Generated Output

Real Target Image

🚀 What I Learned

Conditional GAN working mechanism

Generator vs Discriminator training

U-Net architecture

PatchGAN concept

Adversarial + L1 Loss balancing

Image preprocessing pipeline

🛠 Technologies Used

Python

TensorFlow

NumPy

Matplotlib

📌 Future Improvements

Train for more epochs

Use larger dataset

Experiment with other GAN variants
