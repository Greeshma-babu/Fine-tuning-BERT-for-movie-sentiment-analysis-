# BERT Movie Sentiment Analysis

A simple NLP project that fine-tunes a pretrained **BERT** model for movie review sentiment classification.

## Project Overview

This project uses **BERT (`bert-base-uncased`)** and the **IMDb movie review dataset** to classify movie reviews as:

*  Positive
*  Negative

The pretrained BERT model is fine-tuned on labeled movie reviews and then used to predict the sentiment of new reviews.

## Technologies

* Python
* PyTorch
* Hugging Face Transformers
* Hugging Face Datasets
* BERT
* Scikit-learn

## Project Flow

```text
IMDb Dataset
     ↓
BERT Tokenizer
     ↓
Tokenized Reviews
     ↓
Pretrained BERT
     ↓
Fine-Tuning
     ↓
Sentiment Classification
     ↓
Positive / Negative
```

## Dataset

**IMDb Movie Reviews Dataset**

The dataset contains movie reviews with two sentiment labels:

```text
0 → Negative
1 → Positive
```

## Model

Pretrained model:

```text
bert-base-uncased
```

The model is fine-tuned for binary sentiment classification.

## Installation

Install the required libraries:

```bash
pip install transformers datasets torch scikit-learn accelerate
```
or
```bash
pip install -r requirements.txt
```

## Run the Project

Run:

```bash
python bert_movie_sentiment.py
```

The script will:

1. Download the IMDb dataset
2. Load the BERT tokenizer
3. Tokenize the movie reviews
4. Load pretrained BERT
5. Fine-tune BERT
6. Evaluate the model
7. Save the trained model
8. Test new movie reviews

## Example

Input:

```text
This movie was absolutely fantastic. I loved every minute of it.
```

Output:

```text
Sentiment: POSITIVE
Confidence: 99%
```

Input:

```text
The acting was terrible and the story was extremely boring.
```

Output:

```text
Sentiment: NEGATIVE
Confidence: 99%
```

## Model Output

The trained model is saved in:

```text
bert_movie_sentiment_final/
```

## Evaluation

The model is evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score

## Learning

This project demonstrates:

* BERT
* NLP
* Tokenization
* Transfer Learning
* Fine-Tuning
* Text Classification
* Sentiment Analysis
* Model Evaluation

## Author

**Greeshma Babu**

AI / ML Projects
