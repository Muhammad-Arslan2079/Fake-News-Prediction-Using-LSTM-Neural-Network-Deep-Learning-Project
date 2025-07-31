# 📰 Fake News Prediction Using LSTM Neural Network

This project implements a deep learning model using LSTM (Long Short-Term Memory) to predict fake news based on textual input. It uses a Kaggle dataset combining headlines and article bodies, and applies NLP techniques to clean and preprocess the data before feeding it into an LSTM network.

## 📌 Table of Contents

* [Overview](#overview)
* [Dataset](#dataset)
* [Project Structure](#project-structure)
* [Installation](#installation)
* [Usage](#usage)
* [Model Architecture](#model-architecture)
* [Results](#results)
  



##  Overview

Fake news poses a serious challenge to media and information credibility. This project uses a natural language processing (NLP) approach with LSTM-based deep learning to classify news as real or fake based on its content.

Key components:

* Text preprocessing using NLTK
* Tokenization and padding
* Sequential model using Keras LSTM
* Binary classification



##  Dataset

* **Source**: [Kaggle - Fake News Detection](https://www.kaggle.com/datasets/jruvika/fake-news-detection)
* The dataset contains:

  * `Headline`
  * `Body`
  * `Label` (1 = Fake, 0 = Real)  Assuming this,since I have no information about labels categories as they were already encoded,so I am assuming it as 1=Fake and 0=Authentic, you can change it later on as per you  dataset labels.
* Combined features `Headline` and `Body` into a single `Text` field.



## 🗂 Project Structure

```
Fake_News_Prediction/
├── Fake_News_Prediction_Using_LSTM_Neural_Network_Deep_Learning_Project.ipynb
├── README.md
├── data.csv
└── /models
```



## ⚙️ Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/Fake_News_Prediction.git
cd Fake_News_Prediction
```

2. Install required packages:

```bash
pip install -r requirements.txt
```

3. Set up your Kaggle API credentials to access the dataset:

```bash
# Place your kaggle.json in the working directory
```

---

##  Usage

You can run the notebook using Jupyter:

```bash
jupyter notebook Fake_News_Prediction_Using_LSTM_Neural_Network_Deep_Learning_Project.ipynb
```

Steps performed:

* Data collection via Kaggle API
* Text cleaning and preprocessing
* Tokenization & sequence padding
* LSTM model training
*  Evaluation
*  Building a predictive system

---

##  Model Architecture

* **Embedding Layer**
* **LSTM Layer**
* **Dense Layers**
* **Activation**: Sigmoid for binary classification
* **Dropout**: 0.2 To reduce biasness  by randomly freezing some weights
* **Recurren Dropout**: 0.2 on recurrent hidden layers
* **Loss**: Binary cross entropy for binary classification
* **Metrics**: Accuracy
* **Optimizer**: Adam optimizer
---

##  Results

* Validation Accuracy: *(0.9734)*
* Evaluation Accuracy *(0.9774)* =97%
  
