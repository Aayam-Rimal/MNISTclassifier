# MNIST Digit Classifier (PyTorch)

A simple feedforward neural network for classifying handwritten digits from the MNIST dataset using PyTorch. The project is implemented in a Jupyter notebook for easy experimentation and visualization.

## Overview
- Loads and explores MNIST data.
- Builds a small fully connected neural network.
- Trains the model and reports loss per epoch.
- Evaluates test accuracy.
- Visualizes predictions and misclassifications.

## Repository Structure
- `Digitclassifier.ipynb` — notebook with data loading, model, training, and evaluation.
- `data/` — MNIST dataset files (downloaded via torchvision).
- `environment.yml` — conda environment configuration.

## Requirements
- Python 3.11+
- PyTorch
- torchvision
- matplotlib

## Setup (Conda)
```bash
conda env create -f environment.yml
conda activate mnist
```

## Run
Open the notebook and run all cells:

```bash
jupyter notebook Digitclassifier.ipynb
```

## Model Summary
A simple MLP with:
- Input: 28×28 flattened to 784
- Hidden layers: 128 → 64
- Output: 10 classes

## Results
Typical test accuracy is around **97%+** after a few epochs.

## Notes
- Training and evaluation are performed in the notebook.
- The dataset is downloaded automatically via `torchvision.datasets.MNIST`.

## License
MIT License. See [LICENSE](LICENSE).