# Visual Product Recommender

A deep learning-based system that recommends visually similar fashion products using CNNs and metadata for personalized e-commerce suggestions.

---

## 📌 Overview

This project was built during my master’s at **Duke University – Fuqua School of Business** as part of an advanced analytics course. The goal was to use image data and product metadata to build a visual recommendation system for e-commerce platforms.

## 📂 Dataset

- [Fashion Product Images – Kaggle](https://www.kaggle.com/datasets/paramaggarwal/fashion-product-images-small)
- 44,000+ images with metadata (e.g., `masterCategory`, `subCategory`, `articleType`, `baseColour`, etc.)

## 🧠 Model

- Convolutional Neural Network with:
  - 3 Convolutional layers: 32 → 64 → 128 filters
  - MaxPooling, Dropout, Dense layers
  - Final architecture reached **72.45% accuracy**
- Built using Keras and TensorFlow

## 🛠 Preprocessing

- Label encoding on key categorical features
- Stratified data split for training/validation/testing
- Used `ImageDataGenerator` for augmentation & efficient image loading
- Preprocessed images to 128x128 resolution

## 🔁 Recommendation Engine

- Image embeddings generated via CNN
- Used **Cosine Similarity** to compare input image with dataset
- Returns **Top 5 most visually similar products**

## 🎯 Results

- Final test accuracy: **72.45%**
- Improved over baseline (69.65%) through tuning and regularization
- Effective at capturing visual similarity in fashion products

## 💡 Business Value

- Enhances product discovery and user experience
- Enables cross-selling by showcasing visually similar alternatives
- Can be expanded into hybrid recommenders using behavioral data

## 🖥 Tech Stack

- Python, TensorFlow/Keras
- NumPy, Pandas, Scikit-learn
- Google Colab, Google Drive

## 🛠 Future Work

- Deploy with Streamlit or Flask API
- Add user behavior or session data for hybrid recommendations
- Explore transfer learning with pre-trained CNNs (e.g., ResNet, VGG)

## 📚 Academic Context

This project was completed as part of my Master’s in Quantitative Management – Business Analytics at Duke University.

---

## 📄 License

This project is licensed under the **MIT License** – feel free to use or adapt it with attribution.
