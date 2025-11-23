
#  Image Colorization using GAN (Grayscale → Color)

This project focuses on converting **grayscale images into colored images** using a **Generative Adversarial Network (GAN)**.  
The model is trained on the **CIFAR-10 dataset**, where RGB images are converted to grayscale and then used as inputs to the generator.

---

##  Project Overview

- Converts **black & white images** into **colored images**
- Uses a **Generator–Discriminator GAN architecture**
- Trained on **CIFAR-10**
- Implemented entirely in **Google Colab**
- Produces realistic colored outputs from grayscale inputs

---


##  Model Architecture

### **Generator**
- Takes grayscale (1-channel) input  
- Learns to predict 3-channel RGB output  
- Uses CNN layers, BatchNorm, and ReLU  

### **Discriminator**
- Classifies images as **real (original)** or **fake (generated)**  
- Uses convolutional layers with LeakyReLU  

The system is trained using both:
- **Adversarial loss**
- **L1 reconstruction loss**

---

##  Dataset

**CIFAR-10**  
- 60,000 images (32×32, RGB)  
- Converted to grayscale for training  
- Classes: airplane, car, bird, cat, deer, dog, frog, horse, ship, truck

Dataset Source:  
https://www.cs.toronto.edu/~kriz/cifar.html

---

##  How to Run

1. Open `colorization_gan.ipynb` in Google Colab  
2. Install TensorFlow & dependencies  
3. Run all cells  
4. The model will generate colored images at the end

---

## Sample Results

Generated images from grayscale inputs are placed inside the `sample_outputs/` folder.

---

##  Requirements

- Python 3.x  
- TensorFlow / Keras  
- NumPy  
- Matplotlib  

(All pre-installed in Google Colab)

---

##  Future Improvements
- Train on higher-resolution datasets  
- Add U-Net style skip connections  
- Improve color vibrancy and consistency  

---

##  Acknowledgements
- CIFAR-10 dataset by Alex Krizhevsky  
- TensorFlow/Keras documentation  
- Google Colab platform

---

##  Author
**Ananya Singh**
