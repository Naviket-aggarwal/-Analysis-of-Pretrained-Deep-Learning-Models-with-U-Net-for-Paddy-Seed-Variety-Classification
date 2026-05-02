# 🌾 Paddy Seed Variety Classification using Deep Learning

## 📌 Project Title

**Comparative Analysis of Pretrained Deep Learning Models with U-Net for Paddy Seed Variety Classification**

---

## 🧠 Project Overview

This project focuses on the classification of paddy seed varieties using multiple pretrained deep learning models. A complete pipeline is designed starting from raw image collection to preprocessing, segmentation, and final classification.

The study compares the performance of various models and identifies the most effective architecture for accurate classification.

---

## ⚙️ Methodology

The workflow of the project follows these key steps:

1. **Data Collection**

   * Images of paddy seeds were captured manually
   * Controlled setup using white background and proper lighting
   * Dataset includes 4 varieties:

     * Basmati 1509
     * Basmati 370
     * PR126
     * Pusa Basmati

2. **Background Removal**

   * Applied foreground segmentation using **U2-Net**
   * Removed unnecessary background noise
   * Improved focus on Region of Interest (ROI)

3. **Image Processing**

   * Enhanced:

     * Brightness
     * Contrast
     * Sharpness

4. **Dataset Preparation**

   * Total images: **1600**

     * 400 per class
   * Split ratio:

     * Train: 70%
     * Validation: 20%
     * Test: 10%

5. **Model Training**

   * Training performed on GPU-enabled environment (Google Colab)
   * Number of epochs: 20

---

## 🤖 Models Used

The following pretrained deep learning models were evaluated:

* EfficientNet (EN)
* Inception (IN)
* MobileNet (MN)
* ResNet (RN)
* VGG
* Vision Transformer (ViT)
* DenseNet (DN)

---

## 📊 Results & Analysis

### ✅ Accuracy Comparison

* EfficientNet: **98%** (Best)
* ResNet & VGG: 97%
* DenseNet: 93%
* MobileNet: 91%
* ViT: 86%
* Inception: 80%

---

### 📈 Recall Performance

EfficientNet achieved the highest recall across all classes, with near-perfect detection capability.

---

### 🎯 Precision

EfficientNet maintained the highest precision (~98%), ensuring reliable predictions.

---

### ⚖️ F1-Score

EfficientNet again outperformed all models with the highest balanced performance.

---

## 🏆 Key Outcome

➡️ **EfficientNet emerged as the best-performing model**

* Highest Accuracy
* Highest Precision
* Highest Recall
* Best F1-Score

---

## 📊 Confusion Matrix Insights

* Perfect classification for:

  * Basmati 1509
  * PR126
* Near-perfect classification for:

  * Pusa Basmati (~99.5%)
* Minor misclassification observed in:

  * Basmati 370

---

## 🧪 Dataset Details

* Total Images: **1600**
* Classes: 4
* Data collected manually from local sources
* Background removed using U2-Net

---

## 🛠 Tech Stack

* Python
* TensorFlow / Keras
* OpenCV
* NumPy
* Matplotlib
* Google Colab

---

## ▶️ How to Run

1. Clone the repository
2. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```
3. Open `EfficientNet.ipynb`
4. Run cells sequentially

---

## ⚠️ Note

* Model training was performed on a GPU-enabled system
* Notebook contains results, evaluation metrics, and visualizations

---

## 🚀 Future Scope

* Real-time deployment using IoT devices
* Mobile-based classification system
* Expansion to more crop varieties

---

## 📌 Conclusion

This study demonstrates the effectiveness of pretrained deep learning models for agricultural classification tasks. Among all models tested, **EfficientNet provides the most accurate and reliable performance**, making it a strong candidate for real-world deployment in smart agriculture systems.

---

