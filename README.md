# 🍽️ Food vs. Not Food Text Classification

## 📌 Overview
This project is a text classification model built using Hugging Face's 🤗 transformers library. The model classifies textual data into two categories: **🍕 Food** and **🚫 Not Food**. It utilizes a pre-trained transformer model fine-tuned on a labeled dataset for text classification.

## ✨ Features
- 🚀 **Uses Hugging Face Transformers**: Implements a transformer-based model for text classification.
- 📊 **Fine-tuned on Custom Data**: Trained on a dataset to distinguish between food-related and non-food-related texts.
- ⚡ **Easy-to-Use Pipeline**: Provides a simple way to predict text categories.

## 📂 Dataset
The dataset consists of labeled text examples, where:
- **0️⃣ Label 0**: Not Food 🚫
- **1️⃣ Label 1**: Food 🍽️

## 🛠️ Installation
To set up the environment, install the necessary dependencies:
```bash
pip install transformers datasets torch scikit-learn
```

## 🏋️‍♂️ Training the Model
The model is fine-tuned using the Hugging Face `Trainer` API. The key steps include:
1. 📥 **Loading the dataset**
2. ✂️ **Preprocessing text** using tokenization
3. 🏗️ **Defining the model** using a pre-trained transformer
4. 🎯 **Training and evaluation**

## 🔍 Inference
Once trained, you can use the model to classify new text samples:
```python
from transformers import pipeline

classifier = pipeline("text-classification", model="gokulan006/food101")
text = "This pizza is delicious!"
prediction = classifier(text)
print(prediction)
```

## 📊 Results
The model achieves an accuracy of **X%** on the test dataset (Replace **X%** with actual accuracy from your evaluation).

## 🚀 Future Improvements
- 🏆 Experiment with different transformer architectures.
- 📈 Use larger datasets for better generalization.
- 🎯 Optimize hyperparameters for improved performance.

## 🙌 Credits
- Built using [Hugging Face](https://huggingface.co/) 🤗
- Dataset sourced from [your dataset source] 📊

## 📜 License
This project is for educational purposes only and follows the guidelines of the ZTM course. Redistribution or commercial use may be restricted.

