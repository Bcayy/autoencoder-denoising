# README

## 🧠 Project Title
**Convolutional Denoising Autoencoder for MNIST Digit Restoration**

## 📄 Description of the Files

- `autoencoder_mnist.py`: Main Python script that trains and evaluates the convolutional denoising autoencoder.
- `figures/`: Contains result plots including loss curves and denoised image comparisons.
  - `flowchart.png`: Model architecture overview
  - `denoised_examples.png`: Noisy vs. denoised vs. original images
  - `loss_curve.png`: Training loss over epochs
  - `supp_denoised_1.png`, `supp_denoised_2.png`: Additional visual results for supplementary material
- `main.tex`: Main LaTeX source file for the final report
- `sec/`: Folder containing LaTeX sections (abstract, intro, methods, etc.)
- `main.bib`: Bibliography file
- `ieeenat_fullname.bst`: Bibliography style file
- `Deneme.pdf`: Final project report in CVPR 2025 format
- `poster.pdf`: Project presentation poster (to be added)

## 📦 Required Libraries

Below are the required libraries with their tested versions:

```bash
Python 3.9+
tensorflow==2.13.0
numpy==1.24.3
matplotlib==3.7.1
scikit-image==0.20.0
psutil==5.9.5
```

Install dependencies using:
```bash
pip install -r requirements.txt
```

Alternatively, install manually:
```bash
pip install tensorflow numpy matplotlib scikit-image psutil
```

## 📂 Dataset

- **Dataset**: [MNIST Handwritten Digits Dataset](http://yann.lecun.com/exdb/mnist/)
- **Access via Keras**:
```python
from tensorflow.keras.datasets import mnist
```

No manual download needed — it is automatically fetched using Keras.

## ▶️ How to Run

```bash
python autoencoder_mnist.py
```

### What it does:
- Loads and preprocesses MNIST dataset
- Adds random noise to test images
- Trains convolutional denoising autoencoder
- Saves:
  - `figures/loss_curve.png`
  - `figures/denoised_examples.png`
  - Supplementary denoised outputs
- Reports PSNR and SSIM metrics in console

## ✉️ Author
Burak Akçay  
Bahçeşehir University  
`burak.akcay@bahcesehir.edu.tr`
