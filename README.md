# 📈 SentInvest – AI-Powered Stock Investment Decision Support System

Welcome to **SentInvest**, an AI-driven stock prediction and recommendation system that combines **LSTM-based price forecasting** with **FinBERT-based sentiment analysis** to provide smart investment decisions.

---

## 🚀 Features
- ✅ **LSTM-based Stock Price Prediction**
- ✅ **Real-time Sentiment Analysis** using Financial News
- ✅ **Rule-Based Investment Recommendations** (BUY, SELL, HOLD)
- ✅ **User-Friendly Web Interface with Streamlit**
- ✅ **Dynamic News Scraping** using Google Search and Newspaper3k

---

## 🛠️ Tech Stack
- **Frontend:** Streamlit  
- **Backend:** Python  
- **ML Models:** LSTM (Keras, TensorFlow), FinBERT (Hugging Face)  
- **Data Processing:** Pandas, NumPy, Scikit-Learn  
- **News Scraping:** Googlesearch, Newspaper3k  
- **Visualization:** Streamlit, Matplotlib  

---
⚙️ Installation Guide for SentInvest
Follow these steps to set up and run the SentInvest project locally.

📂 Step 1: Clone the Repository
git clone https://github.com/your-username/SentInvest.git
cd SentInvest

🐍 Step 2: Create a Virtual Environment
python -m venv env

💻 Step 3: Activate the Virtual Environment
For Windows:
.\env\Scripts\activate

For macOS / Linux:
source env/bin/activate

📦 Step 4: Install Required Packages
pip install --upgrade pip
pip install -r requirements.txt

🗂️ Step 5: Project Folder Structure
SentInvest/
│
├── app.py                # Streamlit frontend
├── final_main.py         # Backend processing, LSTM, Sentiment Analysis
├── data.csv              # Stock price data
├── models/               # Trained LSTM models
├── requirements.txt      # Python dependencies
└── README.md             # Project documentation

▶️ Step 6: Run the Application
streamlit run app.py

⚡ The app will open automatically in your default web browser.

🔑 Step 7: Add Hugging Face API Key
Make sure to replace the placeholder:

headers = { "Authorization": "Bearer API" }

👉 Add your actual Hugging Face API token here for FinBERT sentiment analysis to work.

💡 Notes:
Ensure your Python version is 3.8 or higher.

Recommended to use Google Chrome or Firefox for the best Streamlit experience.

If newspaper3k fails to download some articles, re-run the app as some sources may temporarily block requests.

