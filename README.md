# U-Net + MobileNetV2 for Semantic Segmentation

This project implements a semantic segmentation model using a hybrid architecture combining U-Net and MobileNetV2, along with various advanced enhancements like Inception, Attention, Residual, and Squeeze-and-Excitation (SE) modules. It was developed as part of a freelance project to perform instance labeling and mask generation on custom datasets.

## 🔍 Project Overview

- **Base Architecture**: U-Net  
- **Encoder Backbone**: MobileNetV2  
- **Enhancements**:
  - Inception module (for multi-scale context)
  - Attention module (for spatial focus)
  - Residual connections (for gradient flow)
  - SE block (for channel-wise recalibration)

## 📌 Features

- **Custom Dataset Support** (with labeled masks)
- **Mask Generation using Sigmoid Activation**
- **Modular architecture for experimentation**
- **High-resolution segmentation output**
- **Evaluation metrics**: IoU, Dice Score

## 🧠 How It Works

1. **Input Image** → Preprocessing and resizing  
2. **Forward Pass through U-Net + MobileNetV2 Encoder**  
3. **Feature Enhancement** using Inception, Attention, Residual, and SE  
4. **Decoder** reconstructs segmentation map  
5. **Sigmoid Activation** applied on final layer to generate binary masks  
6. **Thresholding** produces final segmentation mask (values ∈ {0, 1})

## 📁 File Structure

├── unet-mobilenetv2.ipynb # Main Jupyter Notebook
├── data/ # Folder for input images and labels
├── models/ # Model definitions (optional if modularized)
├── outputs/ # Folder to save predicted masks
└── README.md


## 🧪 Usage

### 1. Clone the repository

git clone https://github.com/yourusername/unet-mobilenetv2.git
cd unet-mobilenetv2
