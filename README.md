# **Enhancing Face Detection in Low-Light Conditions using Denoising Techniques**

## **Introduction**  
Face detection in low-light environments presents significant challenges due to high levels of noise and loss of key facial features. This research investigates the impact of various noise types on face detection accuracy and evaluates multiple denoising techniques to enhance the performance of face detection models. The goal is to determine which denoising method best preserves facial details while reducing noise interference, thereby improving detection accuracy in real-world low-light scenarios.  

## **Research Focus**  
- **Noise Impact Analysis**: Studying how different types of noise—Gaussian, Poisson, and salt-and-pepper—affect the performance of face detection models.  
- **Denoising Techniques Comparison**: Evaluating traditional and advanced denoising methods, including:  
  - **Median Filtering** (Traditional, spatial domain)  
  - **Non-Local Means (NLM)** (Patch-based)  
  - **Wavelet Transform** (Transform-based)  
  - **DnCNN** (Deep learning-based convolutional neural network)  
- **Performance Evaluation**: Comparing the effectiveness of these denoising techniques using image quality metrics and face detection accuracy.  
- **Dataset**: Utilizing the **Dark Face Dataset**, which contains low-light and noisy face images, ensuring robust testing and validation.  

## **Methodology**  

### **1. Dataset Preprocessing**  
- The **Dark Face Dataset** was selected as it contains real-world low-light images with varying levels of noise.  
- Different types of synthetic noise (Gaussian, Poisson, salt-and-pepper) were added to simulate real-world noise conditions.  

### **2. Application of Denoising Techniques**  
- **Median Filtering**: A simple but effective noise reduction technique using a kernel-based approach.  
- **Non-Local Means (NLM)**: A patch-based filtering method that removes noise while preserving textures.  
- **Wavelet Transform**: A frequency-domain method that decomposes an image into different frequency components for noise removal.  
- **DnCNN (Deep CNN-based Denoising)**: A deep learning-based approach that learns patterns in noise and effectively reconstructs clean images.  

### **3. Face Detection Performance Evaluation**  
- The denoised images were tested using a **face detection model** (pre-trained Haar cascade & deep learning-based models).  
- The impact of denoising was measured using image quality metrics:  
  - **Peak Signal-to-Noise Ratio (PSNR)** – Measures image clarity and noise reduction.  
  - **Structural Similarity Index (SSIM)** – Assesses the structural similarity between original and denoised images.  
  - **Mean Squared Error (MSE)** – Computes the difference between pixel values before and after denoising.  
- The final **face detection accuracy** was recorded after applying each denoising method to determine its effectiveness in restoring facial features.  

## **Findings & Results**  
- **DnCNN outperformed all traditional methods**, showing superior noise reduction and facial feature preservation.  
- **Median Filtering and NLM** were effective against specific noise types but caused slight blurring.  
- **Wavelet Transform** maintained some structural details but was less effective in extreme low-light conditions.  
- **Face detection models showed improved accuracy when using denoised images from DnCNN**, proving its effectiveness in restoring critical features for detection.  

## **Conclusion**  
- **Deep learning-based DnCNN demonstrated the highest effectiveness** in restoring facial features and enhancing face detection accuracy.  
- **Traditional methods like Median Filtering and NLM improved image quality** but had limitations in extreme noise conditions.  
- **Wavelet Transform was effective for structured noise removal**, but its performance varied across images.  
- **Future Scope**: Integrating these techniques into real-time face recognition systems for security and surveillance applications.  

## **Technologies Used**  
- **Image Processing**: OpenCV, scikit-image  
- **Deep Learning**: TensorFlow, Keras (DnCNN model)  
- **Evaluation Metrics**: PSNR, SSIM, MSE  
- **Programming Language**: Python  

## **Installation & Setup**  

### **Prerequisites**  
Ensure you have Python 3.6+ installed and the required dependencies:  
```bash
pip install opencv-python numpy tensorflow keras scikit-image matplotlib
```

### **Clone the Repository**  
```bash
git clone https://github.com/Yashswi-3/enhancing-face-detection-low-light.git  
cd enhancing-face-detection-low-light
```


## **Results & Future Work**  
This study validates **DnCNN’s superior performance in low-light conditions** and highlights the importance of deep learning for image restoration. Future improvements could include optimizing deep models for real-time applications and testing on additional low-light datasets.  

For detailed results, analysis, and code implementation, refer to the **Research Paper** included in this repository.  

## **Contributors**  
- **Yashswi Shukla** - Researcher, Image Processing & Computer Vision  

---
