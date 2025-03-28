# Real vs. Fake Face Detection

## Overview
This project classifies images as either **real or fake** using a deep learning model. It utilizes **EfficientNet-B0** for image classification and is trained on a dataset of real and fake faces. The model is deployed using **Streamlit**, allowing users to upload images and get predictions.

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/your-repo/real-vs-fake-face-detection.git
cd real-vs-fake-face-detection
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

## Model Training
Run the following command to train and evaluate the model:
```bash
python final1.py
```
- Loads dataset from `dl_split` (train, validation, and test folders).
- Uses EfficientNet-B0 with a modified classifier.
- Saves the trained model as `efficientnet_real_fake1.pth`.

## Deployment
Run the Streamlit web app:
```bash
streamlit run app.py
```
- Upload an image (`.jpg`, `.png`, `.jpeg`).
- Click "Detect Face" to see if the face is real or fake.

## Files & Structure
```
.
├── final1.py            # Model training and evaluation script
├── app.py               # Streamlit web app for detection
├── efficientnet_real_fake1.pth  # Trained model
├── requirements.txt     # Python dependencies
```

## Dependencies
- Python 3.x
- PyTorch
- Torchvision
- Streamlit
- NumPy
- Matplotlib
- Pillow

Install them using:
```bash
pip install torch torchvision streamlit numpy matplotlib pillow
```

