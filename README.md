# 🍱 Smart Food Classification & Recipe Assistant

### Empowering Healthy Choices with AI 🍎🤖  

[![Streamlit](https://img.shields.io/badge/Built%20with-Streamlit-ff4b4b?logo=streamlit)](https://streamlit.io/)  [![Made with Python](https://img.shields.io/badge/Made%20with-Python3-yellow.svg)](https://python.org)  [![Model: CNN](https://img.shields.io/badge/Model-CNN-green.svg)](https://keras.io)

---

## Overview

A Deep Learning and NLP-powered web application that classifies food images and recommends recipes using a pre-trained CNN and Hugging Face language models. Built with TensorFlow, Streamlit, and Transformers, this project brings together **computer vision**, **web scraping**, and **generative AI** to deliver intelligent nutrition assistance.

---

## 🚀 Features

- 🖼️ **Food Recognition**
  - Upload a food image and get instant classification using a CNN model trained on diverse food categories.

- 📊 **Deep Learning Model**
  - Utilizes a trained Keras model (`PretrainedModel2.h5`) to identify over 20+ food classes with high accuracy.

- 🌐 **Live Recipe Recommendations**
  - Automatically scrapes the internet for recipes related to the predicted food class using BeautifulSoup.

- 🧠 **AI-Generated Recipe Instructions**
  - Leverages a Hugging Face transformer model to generate natural-language cooking instructions.

- 💡 **User-Friendly Interface**
  - Built with Streamlit for a smooth and interactive experience.

---

## 🧰 Tech Stack

| Component        | Technology                     |
|------------------|---------------------------------|
| Frontend         | Streamlit                      |
| Backend          | Python                         |
| Model            | CNN (Keras, TensorFlow)        |
| NLP Assistant    | Hugging Face Transformers      |
| Scraping         | BeautifulSoup, Requests        |
| Image Handling   | Pillow, OpenCV                 |

---

## 🗂️ Project Structure

```bash
Smart-Food-Recognition-and-Nutrition-Assistant/
│
├── app/
│ ├── PretrainedModel2.h5 # Trained CNN model
│ ├── Classifier_Model.ipynb # Model training notebook
│ ├── hugging_face_model.pyc # (Compiled model file)
│ └── scraper.py # Web scraping for recipes
│
├── streamlit_app.py # Main Streamlit web app
├── requirements.txt # Python dependencies
├── pyproject.toml # Project configuration
```

---

## ⚙️ Setup Instructions

### 🔧 Prerequisites

- Python 3.8+
- pip

### 🛠️ Installation

```bash
git clone https://github.com/btharun03/FoodClassification-main.git
cd FoodClassification-main
pip install -r requirements.txt
```

### ▶️ Run the App

```bash
streamlit run streamlit_app.py
```

- Open your browser at: http://localhost:8501

---

## 🧠 Model Details

- Input: Food image (.jpg, .png, etc.)
- Output: Predicted food class (e.g., apple, mango, bell pepper)
- Architecture: Convolutional Neural Network trained via Keras
- Additional NLP layer: Text generation for recipe steps using AutoModelForCausalLM from Hugging Face

---

## 🎯 Example Use Case

- Upload a photo of a food item.
- The app classifies it using the trained CNN model.
- It scrapes the web for recipes based on the prediction.
- It uses a transformer model to generate personalized cooking instructions.

---

