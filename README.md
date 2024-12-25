# Enhancing Face Detection in Low-Light Conditions - Denoising Techniques

This project explores methods to improve face detection accuracy in low-light conditions by comparing different denoising techniques. The study involves analyzing the impact of various noise types (Gaussian, Poisson, salt-and-pepper) and their effect on the performance of face detection models. The denoising methods evaluated include traditional techniques such as Median Filtering and Non-Local Means (NLM), as well as advanced methods like Wavelet Transform and DnCNN.

## Features
- **Noise Analysis**: Analyzed how different types of noise (Gaussian, Poisson, salt-and-pepper) affect face detection accuracy.
- **Denoising Methods**: Compared various denoising techniques, including Median Filtering, Non-Local Means (NLM), Wavelet Transform, and DnCNN.
- **Performance Metrics**: Used metrics such as PSNR, SSIM, and MSE to evaluate and compare the denoising methods.
- **Dataset**: Used the Dark Face Dataset for testing and validation.

## Technologies Used
- **Image Processing**: OpenCV, scikit-image
- **Deep Learning**: TensorFlow, Keras (DnCNN)
- **Metrics**: PSNR, SSIM, MSE
- **Programming Languages**: Python

## Setup

### Prerequisites
- Python 3.6 or higher
- OpenCV, TensorFlow, Keras, scikit-image, and other required libraries (listed below)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/enhancing-face-detection-low-light.git
   cd enhancing-face-detection-low-light
