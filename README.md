# 🧠 Sentiment Analysis System using Transformers & Traditional NLP

This project is a **Sentiment Analysis System** built using both **traditional NLP techniques (NLTK)** and **modern Transformer-based models (Hugging Face Transformers)**.  
It automatically detects whether a text is **Positive**, **Negative**, or **Neutral**, and visualizes the overall sentiment distribution.

---

## 🌟 Project Overview

This project showcases the difference between:
1. **Traditional NLP sentiment analysis** (rule-based / lexicon-based approach)
2. **Modern Deep Learning approach** using **DistilBERT**, a lightweight Transformer model.

The goal is to demonstrate how **AI models can understand human emotion in text** — useful for applications such as:
- Recruiter chat filtering  
- Social media monitoring  
- Customer feedback analysis  
- Product review insights  

---

## ⚙️ Technologies Used

| Category | Tools & Libraries |
|-----------|------------------|
| Programming Language | Python 3.x |
| NLP Libraries | `nltk`, `transformers` |
| Data Processing | `pandas`, `numpy` |
| Visualization | `matplotlib`, `seaborn` |
| Environment | Jupyter Notebook |

---

## 📂 Project Structure

📦 sentiment-analysis-project/
├── sentiment_analysis.ipynb     # Main notebook
├── data/                        # Dataset folder (if any)
├── requirements.txt             # Dependencies
├── README.md                    # Project documentation
└── output/                      # Result plots or CSVs

---

## 🧩 Step-by-Step Workflow

### 1️⃣ Data Preprocessing
- Load dataset (CSV or manual text input)
- Clean text (lowercase, remove punctuation, stopwords)
- Tokenize and prepare for analysis

### 2️⃣ Sentiment Analysis (Traditional)
- Use **NLTK’s VADER** model
- Classify each sentence into Positive / Negative / Neutral

### 3️⃣ Sentiment Analysis (Transformers)
- Use **Hugging Face’s DistilBERT model**
- Fine-tuned for emotion detection
- Apply `pipeline("sentiment-analysis")` for classification

### 4️⃣ Visualization
Visualize results using **Matplotlib** and **Seaborn**:
- Sentiment distribution chart
- Comparison between old vs modern method

---

## 📊 Example Output

Example of model performance visualization:

| Sentiment | Count |
|------------|--------|
| Positive   | 56%    |
| Neutral    | 32%    |
| Negative   | 12%    |

```python
sns.countplot(data=df, x='sentiment', palette='coolwarm')
plt.title("Sentiment Distribution")
plt.show()

🚀 How to Run This Project
	1. Clone the repository
git clone https://github.com/<your-username>/sentiment-analysis.git
cd sentiment-analysis
  2. Install dependencies
pip install -r requirements.txt
  3. Run Jupyter Notebook
jupyter notebook
  4. 4.	Open sentiment_analysis.ipynb
and run each cell step-by-step.

⸻

💬 Example Use Case

A recruiter system can automatically scan incoming chat messages or application reviews to:
	•	Detect negative tones (e.g., frustration or complaint)
	•	Prioritize positive candidates
	•	Monitor team sentiment over time

This helps companies maintain healthy communication environments powered by AI.

⸻

🌈 Future Improvements
	•	Deploy as Flask web app or Streamlit dashboard
	•	Support multi-language sentiment analysis
	•	Add emotion detection (joy, anger, sadness, etc.)
	•	Integrate with real-time chat systems (Telegram, Slack, etc.)

⸻

👩‍💻 Author

Brielle Alexis Christabel
💡 Passionate about Data Science, AI, and NLP
📍 Project built with guidance and love 💛

⸻

🪶 License

This project is open-source and available under the MIT License.
