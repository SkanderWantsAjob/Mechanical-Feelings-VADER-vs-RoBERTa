# 📖 Overview

This project dives into the duality of sentiment analysis — the symbolic rigidity of **VADER** and the neural subtlety of **RoBERTa** — as they interpret human emotion encoded in Amazon product reviews.

We compare both models across 500 sampled reviews from the **Amazon Review Dataset** available on Kaggle, extract sentiment scores, and visualize how traditional rule-based analysis measures up to modern transformer-based understanding.

---

# 🔍 Features

- Preprocessing and Exploratory Data Analysis (EDA) on Amazon reviews.
- Sentiment scoring using:
  - 🧠 **VADER** — a rule-based model from NLTK.
  - 🤖 **RoBERTa** — transformer-based model fine-tuned for sentiment via HuggingFace.
- Visualization of sentiment trends across review scores.
- Comparative plots of negative, neutral, and positive scores.
- Examples highlighting edge cases and divergence in model outputs.
- Interpretability insights: which reviews *"fool"* which model?

---

# 📁 Dataset

This project uses the **Amazon Review Dataset** from Kaggle, a collection of product reviews across various categories. The dataset contains reviews from real Amazon customers, including text, star ratings, and metadata. For this analysis, only the first **500 entries** are sampled for speed and interpretability. You can access the full dataset [here]([https://www.kaggle.com/datasets/](https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews)).

---

# 🛠️ Tech Stack

- **Python**
- `pandas`, `seaborn`, `matplotlib`
- `nltk` (VADER + POS/NER tagging)
- `transformers` (RoBERTa via HuggingFace)
- `tqdm` for progress bars
- Google Colab / Jupyter-compatible

---

# ▶️ How to Run

1. Clone this repository.
2. Upload your own `Reviews.csv` or use the sample dataset.
3. Run all cells in the provided notebook (`.ipynb`) on Google Colab or Jupyter.
4. Adjust the line `df = df.head(500)` to include more reviews if needed.

---

# 📊 Visuals

Includes:

- Distribution of reviews by star rating
- Compound sentiment vs. review scores (bar plots)
- Side-by-side comparison of VADER and RoBERTa sentiment scores using pairplot

---

# 🔮 Insights

- **VADER** excels in surface-level sentiment but falters in nuance and sarcasm.
- **RoBERTa** is powerful but not immune to misinterpreting domain-specific language or mixed sentiments.
- Some 5-star reviews still contain critical tones, showing a gap between star rating and textual emotion.
