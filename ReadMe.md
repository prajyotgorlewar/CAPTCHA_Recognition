# 🧠 CAPTCHA Recognition Using Deep Learning

## 🚩 Problem Statement

CAPTCHAs (Completely Automated Public Turing test to tell Computers and Humans Apart) are widely used to differentiate between human users and automated bots. However, recognizing and decoding CAPTCHAs using deep learning poses a unique challenge due to distortions, noise, and varying fonts.

The objective of this project is to develop a deep learning model that can accurately recognize and decode multi-character CAPTCHA images using convolutional neural networks (CNNs).

---

## 📖 Project Explanation

This project trains a CNN-based model to solve multi-character CAPTCHA recognition tasks. Each CAPTCHA contains 5 alphanumeric characters, and the model is designed to output one prediction per character.

Key features of the project:
- **Image preprocessing** and one-hot encoding of each character
- **Multi-output model** architecture with separate softmax layers for each character
- **Data augmentation** to improve model generalization
- **Evaluation** of character-level and full-string prediction accuracy

The model architecture includes:
- Multiple convolutional and max pooling layers
- Batch normalization and dropout for regularization
- Five dense output layers (one per character position)
- Categorical cross-entropy loss for each output

---

## 📂 Dataset

The dataset consists of thousands of CAPTCHA images, each containing 5 randomly generated alphanumeric characters. The images are labeled using the text in their filenames.

- Image format: `.png`
- Image size: `160x60 pixels`
- Number of characters: 5 per image
- Classes: 0-9, a-z, A-Z (62 total)

🔗 **Dataset Link**: [CAPTCHA Images Dataset on Kaggle](https://www.kaggle.com/datasets/fournierp/captcha-version-2-images)

---

## 🚀 Future Improvements

- Use a CRNN (CNN + LSTM) architecture for better sequence modeling
- Apply attention mechanisms to focus on character regions
- Convert to real-time CAPTCHA solvers using OCR integration
