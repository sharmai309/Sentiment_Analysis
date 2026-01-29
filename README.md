# Sentiment_Analysis
Mental Health Sentiment Analysis


# Sentiment Analysis of Mental Health Text Data

## 📌 Problem Statement
Understanding emotional tone in mental health–related text can help identify patterns
across different psychological conditions.  
This project applies **sentiment analysis** to labeled mental health statements to
analyze how sentiment varies across conditions such as Depression, Anxiety, and Suicidal ideation.

⚠️ This analysis is **linguistic**, not clinical, and is intended for analytical insights only.

---

## 📊 Dataset
- Size: 53,043 text statements
- Labels (7):
  - Normal
  - Depression
  - Suicidal
  - Anxiety
  - Bipolar
  - Stress
  - Personality Disorder
- Missing statements: 375

**Note:** The dataset is used strictly for educational and analytical purposes.

---

## 🛠 Tools & Technologies
- Python
- Pandas & NumPy
- NLTK (VADER Sentiment Analyzer)
- Matplotlib / Seaborn
- Jupyter Notebook

---

## ⚙️ Methodology
1. Text preprocessing and validation  
2. Sentiment scoring using **VADER**
   - Compound score range: `[-1, 1]`
3. Sentiment classification:
   - Negative: compound < -0.05
   - Neutral: -0.05 ≤ compound ≤ 0.05
   - Positive: compound > 0.05
4. Aggregation of sentiment metrics by mental-health label
5. Visualization and comparative analysis

---

## 📈 Key Results & Insights
- **Depression** and **Suicidal** categories show the strongest negative sentiment
- **Normal** is the only category with a clearly positive average sentiment
- **Anxiety** and **Stress** skew negative but are less extreme
- **Bipolar** and **Personality Disorder** show mixed sentiment with a sizable positive share

### Average Compound Sentiment (Selected)
| Label        | Mean Compound |
|--------------|---------------|
| Normal       | +0.098 |
| Depression  | -0.330 |
| Suicidal    | -0.442 |
| Anxiety     | -0.354 |
| Stress      | -0.239 |

---

## 📊 Visual Outputs
- Distribution of sentiment scores
- Average sentiment by mental-health label
- Label-wise data volume comparison

(Plots included in the repository)

---

## ⚠️ Important Note
This project measures **language sentiment**, not mental health severity.
Positive sentiment may reflect recovery language, optimism, sarcasm,
or quoted speech rather than emotional state.

---

## ▶️ How to Run
```bash
git clone https://github.com/yourusername/sentiment-analysis-mental-health.git
cd sentiment-analysis-mental-health
pip install -r requirements.txt
jupyter notebook
