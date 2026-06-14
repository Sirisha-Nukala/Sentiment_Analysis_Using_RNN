# Sentiment Analysis Using RNN

A deep learning project for classifying IMDB movie reviews as **positive** or **negative** using text preprocessing, TF-IDF vectorization, and a **Recurrent Neural Network (RNN)** implemented with PyTorch.

---

## Project Overview

This project performs sentiment analysis on the IMDB movie reviews dataset to classify reviews into two categories:

* Positive Review → `1`
* Negative Review → `0`

The project covers the complete machine learning pipeline:

* Data preprocessing
* Text cleaning
* Feature extraction
* Model building
* Training
* Evaluation

---

## Features

✔ Text preprocessing and cleaning
✔ HTML tag removal
✔ URL removal
✔ Punctuation removal
✔ Stopword handling
✔ Word stemming
✔ TF-IDF vectorization
✔ Custom RNN implementation using PyTorch
✔ Binary sentiment classification

---

## Tech Stack

* Python
* PyTorch
* Pandas
* NLTK
* Scikit-learn
* NumPy

---

## Dataset

This project uses the **IMDB Movie Reviews Dataset**, a popular dataset for sentiment analysis containing labeled movie reviews.

Dataset labels:

* `1` → Positive sentiment
* `0` → Negative sentiment

---

## Data Preprocessing

Before training the model, text data was cleaned using multiple preprocessing techniques.

### Steps Performed:

1. Removed HTML tags using Regular Expressions
2. Removed URLs
3. Removed punctuation and special characters
4. Tokenized text into words
5. Removed stopwords
6. Applied stemming using Porter Stemmer

These steps help reduce noise and improve model performance.

---

## Feature Engineering

Text data cannot be directly fed into neural networks, so reviews were converted into numerical vectors using **TF-IDF (Term Frequency-Inverse Document Frequency)**.

### TF-IDF Settings

* Maximum Features: `5000`

TF-IDF helps identify important words in reviews while reducing the effect of common words.

---

## Model Architecture

A custom **Recurrent Neural Network (RNN)** was built using PyTorch.

### Architecture:

Input Layer
↓
RNN Layer
↓
Fully Connected Layer
↓
Sigmoid Activation
↓
Output Layer (Binary Classification)

### Hyperparameters

* Hidden Size: `128`
* Number of Layers: `1`
* Epochs: `10`
* Optimizer: Adam
* Loss Function: Binary Cross Entropy Loss (BCELoss)

---

## Training

The model was trained using:

* Forward propagation
* Backpropagation
* Adam optimizer for weight updates

Training was performed for **10 epochs**.

---

## Evaluation

The trained model was evaluated on the test dataset using:

* Accuracy Score

The model predicts whether a movie review expresses positive or negative sentiment.

---

## Project Workflow

1. Load dataset
2. Clean text data
3. Apply preprocessing
4. Convert text into TF-IDF vectors
5. Split data into training and testing sets
6. Build custom RNN model
7. Train model
8. Evaluate performance

---

## Future Improvements

Possible enhancements for this project:

* Replace simple RNN with LSTM or GRU
* Use word embeddings instead of TF-IDF
* Perform hyperparameter tuning
* Improve model accuracy
* Deploy as a web application using Streamlit or Flask

---

## Repository Structure

```bash
Sentiment_Analysis_Using_RNN/
│
├── .gitignore                  # Git ignored files
├── LICENSE                     # MIT License
├── RNN_SentimentAnalysis.ipynb # Complete project notebook
└── README.md                   # Project documentation
```

---

## Author

Developed by **Sirisha Nukala**
