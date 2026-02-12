# Twitter Sentiment Analysis (Naive Bayes From Scratch)

A multiclass Sentiment Analysis model built completely from scratch using the Naive Bayes algorithm in Python.

The model classifies tweets into:

✅ Positive

❌ Negative

➖ Neutral


# 📊 Final Model Performance

Validation Results:

🎯 Accuracy: 96.26%

📌 Precision: 0.9629

📌 Recall: 0.9626

📌 F1-Score: 0.9626

🔎 Per-Class Performance
Sentiment	Precision	Recall	F1-Score	Support
Positive	0.9404	0.9675	0.9537	277
Negative	0.9697	0.9624	0.9660	266
Neutral	0.9785	0.9579	0.9681	285

✔ Very strong balanced performance across all classes
✔ Minimal misclassification

📈 Confusion Matrix Summary
Actual \ Predicted	Positive	Negative	Neutral
Positive	268	5	4
Negative	8	256	2
Neutral	9	3	273

Most predictions fall correctly on the diagonal → indicates high model reliability.

🚀 Features
🔹 Advanced Text Preprocessing

Lowercasing

URL removal

User mention removal

Hashtag cleaning

Negation handling (important for sentiment)

Special character removal

Repeated character normalization

🔹 Feature Engineering

Unigrams

Bigrams (optional)

Stopword removal (important negations preserved)

Porter Stemming

Minimum word frequency filtering

🔹 Model Implementation

Multiclass Naive Bayes (built from scratch)

Log probabilities to prevent underflow

Laplace smoothing

Log prior calculation

🔹 Evaluation

Accuracy

Precision

Recall

F1-Score

Per-class metrics

Confusion Matrix

Classification Report

📂 Dataset

Training Samples: 60,981

Validation Samples: 828

Training Distribution:

Negative: 22,312

Positive: 20,618

Neutral: 18,051


Mathematical Foundation

The model is based on the Naive Bayes Theorem:

Naive Bayes Formula
P(Class | Words) ∝ P(Class) × ∏ P(Word | Class)


This means:

P(Class | Words) → Probability of a class given the words

P(Class) → Prior probability of the class

P(Word | Class) → Likelihood of each word given the class

The product (∏) multiplies probabilities of all words

Log Probability Version (Used in Code)

To prevent numerical underflow, we use log probabilities:

log P(Class | Words) = log P(Class) + Σ log P(Word | Class)

Laplace Smoothing

To avoid zero probabilities:

P(word | class) = (count(word) + 1) / (total_words + V)


Where:

count(word) → Number of times the word appears in that class

total_words → Total words in that class

V → Vocabulary size

+1 → Laplace smoothing
🏆 Highlights

✔ 96.26% Accuracy
✔ Built fully from scratch (no prebuilt Naive Bayes used)
✔ Bigram feature support
✔ Clean modular code structure
✔ Strong generalization on validation set
