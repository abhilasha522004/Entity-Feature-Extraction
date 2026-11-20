# 📦 Image-Based Entity Value Extraction

## 🎯 Project Overview
This project focuses on extracting entity values 📊 (such as **weight, volume, dimensions**) from product images using **Machine Learning** techniques. The approach involves:

- 🧠 **Optical Character Recognition (OCR)** for textual information
- 🖼️ **Convolutional Neural Networks (CNN)** for visual features

Both techniques work together to improve entity extraction accuracy. 🚀

---

## ⚙️ Setup and Installation
1. 📥 **Clone the repository:**
   ```bash
   git clone https://github.com/abhilasha522004/Entity-Feature-Extraction.git
   cd Entity-Feature-Extraction
   ```
2. 📦 **Install dependencies** (Python 3.9+ and the [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) engine are required):
   ```bash
   pip install torch torchvision scikit-learn pandas numpy opencv-python pytesseract pillow matplotlib seaborn tqdm
   ```

---

## 🚀 Pipeline
Run the scripts in this order:

| Step | Script | What it does |
|---|---|---|
| 1 | `data-preparation.py` | Downloads product images and builds the train/validation split |
| 2 | `label-preprocessing.py` | Normalizes entity values and units |
| 3 | `image-preprocessing.py` | Resizes and cleans images for OCR and the CNN |
| 4 | `ocr-feature-extraction.py` | Extracts text from images with Tesseract |
| 5 | `cnn-feature-extraction.py` | Extracts visual features with a pretrained CNN |
| 6 | `model-development.py` | Trains the hybrid OCR + CNN model |
| 7 | `performance-optimization.py` | Tunes the model |
| 8 | `error-analysis.py` | Confusion matrix and classification report |
| 9 | `prediction-output-generation.py` | Generates predictions for the test set |

A full write-up of the approach is in `Image_Based_Entity_Extraction_Project.docx`.

---

## 🧩 Model Architecture
The hybrid architecture consists of:

- 🧠 **OCR Branch:** Embedding layer ➡️ LSTM
- 🖼️ **CNN Branch:** Pre-extracted features processed by fully connected layers
- 🔗 **Combined Output:** Concatenated features passed through fully connected layers

---

## 📊 Performance Metrics
- ✅ **Validation Accuracy:** **87%**
- 📈 **F1 Score:** **0.85**

---

## 📈 Future Improvements
- 🎭 Implement **data augmentation** techniques
- 🔍 Explore **advanced OCR methods**
- 🛠️ Fine-tune hyperparameters using **Bayesian Optimization**

---

## 📞 Contact
For any questions or issues, please feel free to:
- 🐙 Open an **issue** in the GitHub repository
- 📧 Reach out via email

Thank you for checking out the project! 🎉
