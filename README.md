# Klasifikasi-Gambar

# Rice Image Classification using CNN

This project builds a Convolutional Neural Network (CNN) to classify rice grain images into five categories: **Arborio, Basmati, Ipsala, Jasmine, and Karacadag**.

## 📁 Dataset

Dataset: [Rice Image Dataset on Kaggle](https://www.kaggle.com/datasets/muratkokludataset/rice-image-dataset)  
Each class contains **15,000 images**, with uniform size and similar backgrounds.

## 🧪 Data Split

The dataset is split as follows:

- **Training**: 60%
- **Validation**: 20%
- **Test**: 20%

The images are resized to `150x150` and normalized (pixel values scaled between 0 and 1).

## 🔧 Preprocessing

- Resizing to `(150, 150)`
- Normalization (pixel values scaled to [0, 1])
- Data Augmentation using:
  - Random rotation
  - Horizontal flip
  - Zoom
  - Width & height shift

## 🧠 Model Architecture (CNN)

- 3 Convolutional layers + MaxPooling
- Flatten layer
- Fully connected Dense layers
- Dropout for regularization
- `softmax` activation on output layer

Optimizer: `Adam`  
Loss: `categorical_crossentropy`  
Metrics: `accuracy`

## 📈 Training Results

| Metric      | Value    |
|-------------|----------|
| Train Acc   | 0.9842       |
| Val Acc     | 0.9899     |
| Test Acc    | 0.9904      |
| Loss        | 0.0302       |


Training graphs are included in the notebook.
