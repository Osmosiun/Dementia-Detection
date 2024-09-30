# Predicting Dementia Using High-Fidelity MRI: An Empirical Analysis of Diffusion, Autoencoders, and Adversarial Deep Learning Models

This repository contains the implementation of my paper: **"[An Empirical Analysis of Diffusion, Autoencoders, and Adversarial Deep Learning Models for Predicting Dementia Using High-Fidelity MRI](https://doi.org/10.1109/ACCESS.2024.3354724)**".

## Abstract

This study explores cutting-edge computational technologies and intelligent methods to create realistic synthetic data, focusing on dementia-centric Magnetic Resonance Imaging (MRI) scans related to Alzheimer’s and Parkinson’s diseases. The research delves into Generative Adversarial Networks (GANs), Variational Autoencoders, and Diffusion Models, comparing their efficacy in generating synthetic MRI scans. Using datasets from Alzheimer’s and Parkinson’s patients, the study reveals intriguing findings. 

- In the Alzheimer dataset, diffusion models produced non-dementia images with the lowest Frechet Inception Distance (FID) score at 92.46, while data-efficient GANs excelled in generating dementia images with an FID score of 178.53.
- In the Parkinson dataset, data-efficient GANs achieved remarkable FID scores of 102.71 for dementia images and 129.77 for non-dementia images.

The study also introduces a novel aspect by incorporating a classification study, validating the generative metrics. DenseNets, a deep learning architecture, exhibited superior performance in disease detection compared to ResNets. Training both models on images generated by diffusion models further improved results, with DenseNet achieving accuracies of 80.84% and 92.42% in Alzheimer’s and Parkinson’s disease detection, respectively. The research not only presents innovative generative architectures but also emphasizes the importance of classification metrics, providing valuable insights into the synthesis and detection of neurodegenerative diseases through advanced computational techniques.

## Generative Models

We used four generative models to produce training images:
1. Variational Autoencoders
2. Generative Adversarial Network
3. Data Efficient GAN
4. Diffusion Models

These generative models were trained to produce synthetic images, which were then combined with the original images to train classification models.

## File Descriptions

- **Classification_Model_Training_and_Inference.ipynb**: Training and inference of classification models like ResNet and DenseNet.
- **Data_Efficient_GAN_Training.ipynb**: Training of data efficient GANs.
- **Diffusion_Model_Training.ipynb**: Training of diffusion models.
- **GAN_Training.ipynb**: Training of GAN.
- **VAE_Training.ipynb**: Training of Variational Autoencoders.

