# Google Play Review Sentiment Analyzer

A web-based application that fetches real user reviews from any Google Play Store app and analyzes them using a transformer-based sentiment analysis model from Hugging Face.

## Features

- Extracts recent reviews from a Google Play Store app.
- Analyzes sentiments (positive/negative) using `siebert/sentiment-roberta-large-english`.
- Calculates sentiment distribution and makes download-worthiness recommendations.
- Clean, responsive frontend (HTML + JS).
- Backend powered by Flask and exposed using Ngrok.

---

## Tech Stack

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python (Flask)
- **NLP Model**: Hugging Face Transformers
- **Data Source**: `google-play-scraper`
- **Deployment**: `pyngrok` for local-to-public testing

---

## Installation

### 1. Clone the repository
```bash
git clone https://github.com/coderSagnikDS/google-play-app-review-sentiment-analyser.git
cd google-play-sentiment-analyzer
```
### 2. Set up Python environment
Make sure you have latest Python installed. It's recommended to use a virtual environment:
```bash
pip install -r requirements.txt
```
### 3. Set up Ngrok (optional for local public access)
Create an account at https://ngrok.com/ and get your auth token.
In your Python code (before starting the app), add:
```bash
from pyngrok import ngrok
ngrok.set_auth_token("your_token_here")
```
### 4. Run the Flask app
```bash
python app.ipynb
```

Your app will start at http://localhost:5000 and also provide a public ngrok URL.
Copy the public URL and paste it in Line 100 in my html code
(Update in progress to fix this)

---

## 📈 How It Works
#### 1.Paste a valid Google Play Store app link.
#### 2.Click "Generate Reviews" to view recent user reviews.
#### 3.Click "Generate Sentiment" to analyze the sentiment of those reviews.
#### 4.See a summary of sentiment percentages and a final recommendation.
