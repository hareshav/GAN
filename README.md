
# Fashion MNIST GAN

This project implements a Generative Adversarial Network (GAN) using PyTorch to generate synthetic fashion images based on the Fashion MNIST dataset.

## 🧠 Project Overview

Generative Adversarial Networks (GANs) consist of two neural networks, the **Generator** and the **Discriminator**, which compete in a zero-sum game. The Generator tries to create realistic fashion images, while the Discriminator attempts to distinguish between real and fake images.

This project:
- Loads and preprocesses the Fashion MNIST dataset
- Defines and trains a Generator and Discriminator model
- Visualizes synthetic fashion images created by the trained GAN

## 📁 Files

- `GANfashion.ipynb` - Main notebook containing all the code for data loading, model definition, training, and visualization.
- `README.md` - Project documentation.

## 📦 Requirements

Install the following Python libraries:

```bash
pip install torch torchvision matplotlib numpy
```

## 🚀 How to Run

1. Clone this repository or download the notebook.
2. Install dependencies using pip (see above).
3. Open `GANfashion.ipynb` in Jupyter Notebook or Google Colab.
4. Run the cells step by step to train the GAN and visualize results.

## 📊 Results

The Generator learns to produce realistic fashion items like shirts, sneakers, bags, etc., over multiple epochs. Below is a sample output after training:

*Example output images are visualized in the notebook.*

## 🔧 Model Details

### Generator
- Input: Random noise vector (latent space)
- Layers: Fully connected layers + BatchNorm + ReLU
- Output: 28x28 image with Tanh activation

### Discriminator
- Input: 28x28 image
- Layers: Fully connected layers + LeakyReLU
- Output: Probability (real or fake) via Sigmoid

## 📚 Dataset

[Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist) is a dataset of Zalando's article images consisting of 28x28 grayscale images of 10 fashion categories.

## 📈 Training

- Loss Function: Binary Cross Entropy
- Optimizer: Adam
- Epochs: Configurable (typically 50+ recommended)

## 🤖 Author
Haresh A V
This project was developed as part of an exploration into generative deep learning models. Contributions include:
- Data preprocessing
- Model architecture design
- Training loop and performance evaluation

