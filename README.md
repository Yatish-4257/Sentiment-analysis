# Twitter Sentiment Analysis (Naive Bayes From Scratch)

A multiclass Sentiment Analysis model built completely from scratch using the Naive Bayes algorithm in Python.

The model classifies tweets into:

✅ Positive

❌ Negative

➖ Neutral


# 📊 Final Model Performance

Validation Results:

🎯 Accuracy: 96.26%

 Precision: 0.9629

 Recall: 0.9626

 F1-Score: 0.9626



✔ Very strong balanced performance across all classes
✔ Minimal misclassification

# Confusion Matrix Summary
Actual \ Predicted	Positive	Negative	Neutral
Positive	268	5	4
Negative	8	256	2
Neutral	9	3	273

Most predictions fall correctly on the diagonal → indicates high model reliability.

# Features
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

# Dataset

Training Samples: 60,981

Validation Samples: 828

Training Distribution:

Negative: 22,312

Positive: 20,618

Neutral: 18,051


# Highlights

✔ 96.26% Accuracy
✔ Built fully from scratch (no prebuilt Naive Bayes used)
✔ Bigram feature support
✔ Clean modular code structure
✔ Strong generalization on validation set
