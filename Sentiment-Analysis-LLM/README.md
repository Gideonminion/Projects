# Sentiment-Analysis-LLM
# Google Play App Review Sentiment Analysis using BERT

This project demonstrates how to perform sentiment analysis on Google Play app reviews using the BERT (Bidirectional Encoder Representations from Transformers) model.

## Project Overview

The goal of this project is to classify app reviews into three sentiment categories: negative, neutral, and positive. This is achieved by fine-tuning a pre-trained BERT model on a dataset of Google Play app reviews.

## Dataset

The dataset used in this project is a collection of Google Play app reviews, which can be downloaded from the following links:
https://drive.google.com/uc?id=1zdmewp7ayS4js4VtrJEHzAheSW-5NBZv

## Methodology

1. **Data Preprocessing:** The app reviews are preprocessed by tokenizing the text using the BERT tokenizer and converting the text into numerical representations.
2. **Model Building:** A pre-trained BERT model is fine-tuned for sentiment classification. The model consists of a BERT base model followed by a classification layer.
3. **Model Training:** The model is trained on the preprocessed dataset using the AdamW optimizer and a linear learning rate scheduler.
4. **Model Evaluation:** The trained model is evaluated on a held-out test set using metrics such as accuracy and confusion matrix.
5. **Prediction:** The model can be used to predict the sentiment of new app reviews.

## Requirements

- Python 3.7 or higher
- PyTorch
- Transformers library
- Pandas
- NumPy
- Scikit-learn
- Seaborn
- Matplotlib

## Results

The model achieved an accuracy of approximately 89% on the test set.

## Future Work

- Experiment with different BERT model architectures.
- Fine-tune the model on a larger dataset.
- Explore other sentiment analysis techniques.
