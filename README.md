# Autoencoder and Variational Autoencoder (VAE) for Image Reconstruction and Generation

## 📌 Project Overview

This project implements and compares an **Autoencoder (AE)** and a **Variational Autoencoder (VAE)** for image reconstruction and generation using the MNIST handwritten digits dataset.

Both models learn a compressed representation of images and use it to reconstruct images. The VAE can also generate new images by sampling from a learned latent probability distribution.

## 🎯 Objectives

- Implement an Autoencoder and a Variational Autoencoder.
- Reconstruct handwritten digit images.
- Generate new images using learned latent representations.
- Compare reconstruction quality and model performance.
- Visualize and analyze the results.

## 🛠️ Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Pandas
- Scikit-learn
- Jupyter Notebook / Google Colab

## 📂 Dataset

**MNIST Handwritten Digits Dataset**

- 60,000 training images
- 10,000 testing images
- Grayscale images of size 28 × 28 pixels
- Ten digit classes (0–9)

The images are normalized to the range [0, 1] and flattened into 784-dimensional vectors for model training.

## 🧠 Models Implemented

### 1. Autoencoder (AE)

The Autoencoder consists of two components:

- **Encoder:** Compresses the input image into a lower-dimensional latent representation.
- **Decoder:** Reconstructs the original image from the latent representation.

The model is trained using binary cross-entropy loss.

### 2. Variational Autoencoder (VAE)

The VAE learns a probability distribution in the latent space using a mean and log-variance.

Its training objective combines:

- **Reconstruction loss:** Measures how closely the output matches the input.
- **KL divergence loss:** Encourages the learned latent distribution to remain close to a standard normal distribution.

The reparameterization trick enables sampling during training.

## ⚙️ Project Workflow

1. Import libraries and load the MNIST dataset.
2. Preprocess and normalize the images.
3. Build and train the Autoencoder.
4. Build and train the Variational Autoencoder.
5. Reconstruct test images using both models.
6. Generate new images from latent representations.
7. Evaluate reconstruction quality using Mean Squared Error (MSE).
8. Visualize results and compare both models.

## 📊 Performance Evaluation

The models are compared using:

- Reconstruction quality
- Mean Squared Error (MSE)
- Training loss
- Visual quality of generated images
- Diversity of generated images

**Expected observation:** The Autoencoder may produce sharper reconstructions, while the VAE provides a more structured latent space that supports sampling and generating new images. Actual results depend on training settings and should be evaluated from the notebook outputs.

## 🚀 How to Run

### Option 1: Google Colab

1. Download the notebook from this repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Upload `Autoencoder_VAE_Image_Reconstruction_Generation.ipynb`.
4. Run all cells in order.

### Option 2: Jupyter Notebook

Install the required libraries:

```bash
pip install tensorflow numpy matplotlib scikit-learn pandas jupyter
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open the notebook and run all cells.

## 📁 Project Structure

```text
Autoencoder-VAE-Image-Reconstruction/
│
├── Autoencoder_VAE_Image_Reconstruction_Generation.ipynb
└── README.md
```

## ✅ Results

The notebook displays:

- Sample MNIST images
- Autoencoder reconstructions
- VAE reconstructions
- Images generated from latent representations
- Training loss curves
- MSE-based reconstruction comparison
- A summary comparison table

## 🔮 Future Improvements

- Experiment with the Fashion-MNIST dataset.
- Test different latent-space dimensions.
- Improve generated image quality through hyperparameter tuning.
- Explore convolutional Autoencoders and VAEs.
- Compare additional image-quality metrics.

## 👩‍💻 Author

**Tanuja Nikam**

## 📄 License

This project is intended for educational and academic purposes.
