# VQ-VAE Implementation on CIFAR-10 and LibriSpeech ASR Corpus

This repository contains an implementation of the **Vector Quantized Variational Autoencoder (VQ-VAE)** based on the paper [Neural Discrete Representation Learning](https://arxiv.org/abs/1711.00937) by Aaron van den Oord, Oriol Vinyals, and Koray Kavukcuoglu. The implementation is applied to two datasets:
- **CIFAR-10**: for modeling image data.
- **LibriSpeech ASR Corpus**: for modeling audio data.

## Overview

The VQ-VAE model is a generative model that learns discrete latent representations, overcoming challenges such as posterior collapse in traditional VAEs. By combining the variational autoencoder framework with vector quantization, VQ-VAE learns high-quality discrete latent spaces and pairs them with powerful autoregressive priors for tasks such as image and speech generation.

Key features of this implementation include:
- Discrete latent variable representation.
- Prevention of posterior collapse.
- Integration with autoregressive priors (e.g., PixelCNN for images, WaveNet for audio).

## Repository Structure

```plaintext
├── data/                   # Scripts for downloading and processing CIFAR-10 and LibriSpeech datasets
├── models/                 # Implementation of VQ-VAE, PixelCNN, and WaveNet
├── notebooks/              # Jupyter notebooks for visualizations and experiments
├── results/                # Generated results (reconstructed images/audio, loss curves, etc.)
├── utils/                  # Utility scripts for training, evaluation, and visualization
├── main.py                 # Main script for training and evaluation
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation
