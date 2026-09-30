# BERT Fine-Tuning for Movie Sentiment Analysis

An NLP project that fine-tunes a pre-trained **BERT (Bidirectional Encoder Representations from Transformers)** model for binary sentiment classification of movie reviews.

The project demonstrates how **Transfer Learning and Transformer-based NLP** can be used to understand the sentiment expressed in natural-language movie reviews.

##  Project Overview

The model is trained to classify movie reviews into two categories:

*  **Positive** — The review expresses a positive opinion.
*  **Negative** — The review expresses a negative opinion.

Instead of training an NLP model from scratch, this project uses a pre-trained BERT model and fine-tunes it on a movie-review dataset.

### Example

**Input:**

> "This movie was absolutely fantastic. The story, acting, and direction were excellent."

**Prediction:**

```text
Sentiment: Positive
Confidence: 98.7%
```

**Input:**

> "The movie was boring and the story was poorly written."

**Prediction:**

```text
Sentiment: Negative
Confidence: 97.4%
```

##  How BERT Fine-Tuning Works

The project follows the following pipeline:

```text
Movie Reviews
      ↓
Text Preprocessing
      ↓
BERT Tokenizer
      ↓
Token IDs + Attention Masks
      ↓
Pre-trained BERT Model
      ↓
Fine-Tuning
      ↓
Sentiment Classification
      ↓
Positive / Negative
```

BERT already contains knowledge learned from large-scale text during pre-training. Fine-tuning adapts this knowledge to the specific task of movie sentiment classification.

##  Technologies Used

* Python
* PyTorch
* Hugging Face Transformers
* Hugging Face Datasets
* BERT
* Scikit-learn
* Pandas
* NumPy
* Matplotlib
* Jupyter Notebook / VS Code

## Training Process

The main steps are:

1. Load the movie-review dataset.
2. Clean and prepare the text data.
3. Load the pre-trained BERT tokenizer.
4. Tokenize the reviews.
5. Create attention masks.
6. Load a BERT model with a sequence-classification head.
7. Fine-tune BERT using the labeled reviews.
8. Evaluate the model on unseen data.
9. Save the trained model and tokenizer.
10. Use the trained model to predict sentiment for new reviews.

##  Model Evaluation

The model can be evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix

Example evaluation output:

```text
Accuracy  : XX.XX%
Precision : XX.XX%
Recall    : XX.XX%
F1 Score  : XX.XX%
```

The actual values depend on the dataset, preprocessing, BERT checkpoint, hyperparameters, and training configuration.

##  Prediction

After training, the model can classify new movie reviews.

```text
Enter movie review:
"The movie was amazing and the performances were excellent."

Prediction:
Positive

Confidence:
98.7%
```

##  Project Structure

```text
BERT-Movie-Sentiment-Analysis/
│
├── data/
│   └── movie_reviews.csv
│
├── models/
│   └── bert_sentiment/
│
├── notebooks/
│   └── bert_sentiment_analysis.ipynb
│
├── train.py
├── predict.py
├── requirements.txt
├── README.md
└── .gitignore
```

##  Installation

Clone the repository and install the required dependencies:

```bash
git clone <your-repository-url>
cd BERT-Movie-Sentiment-Analysis

pip install -r requirements.txt
```

```bash
python train.py
```

```bash
python predict.py
```

##  Author
Greeshma Babu

