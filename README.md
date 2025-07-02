# 📱 Google Play Review Sentiment Analyzer

A web-based application that fetches real user reviews from any Google Play Store app and analyzes them using a transformer-based sentiment analysis model from Hugging Face.

## 🚀 Features

- 🔍 Extracts recent reviews from a Google Play Store app.
- 🤖 Analyzes sentiments (positive/negative) using `siebert/sentiment-roberta-large-english`.
- 📊 Calculates sentiment distribution and makes download-worthiness recommendations.
- 🌐 Clean, responsive frontend (HTML + JS).
- ⚙️ Backend powered by Flask and exposed using Ngrok.

---

## 📸 Screenshot

![App Screenshot](https://i.imgur.com/your-screenshot-placeholder.png) <!-- optional -->

---

## 🛠 Tech Stack

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python (Flask)
- **NLP Model**: Hugging Face Transformers
- **Data Source**: `google-play-scraper`
- **Deployment**: `pyngrok` for local-to-public testing

---

## 📦 Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/google-play-sentiment-analyzer.git
cd google-play-sentiment-analyzer
