🧠 Twitter Sentiment Analysis (Naive Bayes From Scratch)

A multiclass Sentiment Analysis model built completely from scratch using the Naive Bayes algorithm in Python.

The model classifies tweets into:

✅ Positive

❌ Negative

➖ Neutral

📊 Final Model Performance

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


Mathematical Background

Naive Bayes Formula:

𝑃
(
𝐶
𝑙
𝑎
𝑠
𝑠
∣
𝑊
𝑜
𝑟
𝑑
𝑠
)
∝
𝑃
(
𝐶
𝑙
𝑎
𝑠
𝑠
)
×
∏
𝑃
(
𝑊
𝑜
𝑟
𝑑
∣
𝐶
𝑙
𝑎
𝑠
𝑠
)
P(Class∣Words)∝P(Class)×∏P(Word∣Class)

To avoid numerical underflow:

Log probabilities are used

Laplace smoothing applied:

𝑃
(
𝑤
𝑜
𝑟
𝑑
∣
𝑐
𝑙
𝑎
𝑠
𝑠
)
=
𝑐
𝑜
𝑢
𝑛
𝑡
(
𝑤
𝑜
𝑟
𝑑
)
+
1
𝑡
𝑜
𝑡
𝑎
𝑙
_
𝑤
𝑜
𝑟
𝑑
𝑠
+
𝑉
P(word∣class)=
total_words+V
count(word)+1
	​


Where:

V = Vocabulary size

🏆 Highlights

✔ 96.26% Accuracy
✔ Built fully from scratch (no prebuilt Naive Bayes used)
✔ Bigram feature support
✔ Clean modular code structure
✔ Strong generalization on validation set
