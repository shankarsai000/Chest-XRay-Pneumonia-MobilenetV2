# Chest X-Ray Pneumonia Classification 🫁

![Python](https://img.shields.io/badge/Python-3.11-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.14-green)
![GitHub Repo](https://img.shields.io/badge/GitHub-Repo-black)

---

## Overview
This project classifies **chest X-ray images** into **Pneumonia** or **Normal** using **MobileNetV2** with transfer learning. It leverages deep learning to assist in rapid and automated pneumonia detection.

---

## Dataset
- Source: [Chest X-Ray Pneumonia Dataset on Kaggle](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia)  
- Contains labeled X-ray images for training, validation, and testing.  

---

## Model
- **Architecture:** MobileNetV2 (pre-trained on ImageNet)  
- **Training:** Fine-tuned with chest X-ray images  
- **Output:** Binary classification – Pneumonia / Normal  

> The trained model file is large and not included in the repo.

**Download Trained Model:** [Google Drive Link](https://drive.google.com/file/d/1Hq4Xv9AkDHZZz42BrFxpWU_wnHNTu3nD/view?usp=drive_link)

---

## Usage

1. **Open Notebook**
   - Open `PneumoniaDetection.ipynb` in Kaggle or Jupyter.
2. **Load Model**
   - Use the Drive link to download the model via `gdown`:
   ```python
   !pip install gdown
   import gdown

   url = 'https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia'
   output = 'mobilenetv2_pneumonia.h5'
   gdown.download(url, output, quiet=False)
3)Upload X-ray Image

*Follow the notebook cell to upload your image.

4)Run Prediction

The model will classify the image as Pneumonia or Normal.

Folder Structure:
bash
Copy code
Chest-XRay-Pneumonia-MobilenetV2/
├── PneumoniaDetection.ipynb   # Notebook for training & prediction
├── README.md                  # Project description
├── mobilenetv2_pneumonia.h5   # Trained model (download via Drive)
Notes
1)Ensure uploaded images are grayscale or RGB and roughly 224x224 pixels.

2)The notebook is ready for Kaggle Notebooks or local Jupyter environment.

3)Model training details are included in the notebook for reference.

