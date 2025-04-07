# VAE Symmetries Assignment for GSoC End-to-End Deep Learning Projects @ ML4SCI

## Overview
This repository contains a Variational Autoencoder (VAE) model for learning symmetries in scientific data. The project is developed as part of the GSoC End-to-End Deep Learning Projects at ML4SCI.

## Getting Started
The provided Jupyter Notebook can be run directly. Pretrained models are available for evaluation and further experimentation.

### Best Models
- **vae3.pth** (Trained for 10 epochs)
- **vae3_40.pth** (Trained for 40 epochs)

- Other models for MLP, generators and classifier oracle are given in the models folder.

Additional models may be used alongside `vae3.pth` to compare and analyze performance.

## Hyperparameters

### VAE Model
```python
vae = VAE(latent_dim=32).to(device)
optimizer = optim.Adam(vae.parameters(), lr=1e-3)
epochs = 10 to 30
```

#### VAE Loss Parameters:
- **Beta** = 1.0
- **Gamma** = 12.5
- **Delta** = 0.5

### Latent Supervised MLP
- **Latent Dimension** = 32
- **Epochs** = 10

### Oracle & Generator
- **Oracle Dimensions** = 32
- **Generator Dimensions** = 32
- **Number of Generators** = 3

### Visualization
- **Epsilon** = 0.3 - 0.5

## Usage
1. Load the notebook and run all cells.
2. Use the provided pretrained models for evaluation or retrain using the specified hyperparameters.
3. Experiment with different visualization epsilon values for better interpretability.

## Acknowledgment
This project is developed under ML4SCI as part of GSoC's deep learning initiatives. Special thanks to the contributors and mentors involved in the project.

