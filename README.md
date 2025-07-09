# 📈 SentInvest – AI-Powered Stock Investment Decision Support System

Welcome to **SentInvest**, an AI-driven stock prediction and recommendation system. It combines **LSTM-based stock price forecasting** and **FinBERT-powered financial sentiment analysis** to offer intelligent investment guidance.

---

## 🚀 Features
- ✅ **LSTM-Based Stock Price Prediction**  
- ✅ **Financial News Sentiment Analysis** using [FinBERT](https://huggingface.co/ProsusAI/finbert)  
- ✅ **Rule-Based Investment Recommendations** (BUY / SELL / HOLD)  
- ✅ **User-Friendly Web Interface** powered by Streamlit  
- ✅ **Live News Scraping** via Google Search + Newspaper3k  
- ✅ **Error-Resilient Workflow** with logging and feedback

---

## 🛠️ Tech Stack

| Layer       | Tools/Libraries                                                                 |
|-------------|----------------------------------------------------------------------------------|
| **Frontend**| Streamlit                                                                       |
| **Backend** | Python, Keras, TensorFlow                                                       |
| **ML Models** | LSTM for price forecasting, FinBERT for sentiment analysis (via Hugging Face) |
| **Data**    | Pandas, NumPy, MinMaxScaler, CSV Stock Data                                     |
| **Scraping**| googlesearch-python, newspaper3k                                                |
| **Utils**   | dotenv, joblib, matplotlib, textwrap, datetime                                  |

---

```markdown
# SentInvest

SentInvest is a sentiment analysis tool designed to analyze stock market trends using natural language processing (NLP) techniques. It leverages the FinBERT model to assess sentiment from financial news articles and historical stock price data.

## ⚙️ Installation Guide

Follow the steps below to set up and run the **SentInvest** project locally.

### 📂 Step 1: Clone the Repository
```bash
git clone https://github.com/your-username/SentInvest.git
cd SentInvest
```

### 🐍 Step 2: Create a Virtual Environment
```bash
python -m venv env
```

### 💻 Step 3: Activate the Virtual Environment
For Windows:
```bash
.\env\Scripts\activate
```

For macOS / Linux:
```bash
source env/bin/activate
```

### 📦 Step 4: Install Required Packages
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### 🔑 Step 5: Add Hugging Face API Token
Create a `.env` file in the root directory and paste your token like this:
```env
HF_TOKEN=your_huggingface_api_token
```
This token is used to authenticate requests to FinBERT via Hugging Face.

### 🗂️ Project Folder Structure
```bash
SentInvest/
│
├── app.py             # Streamlit frontend
├── main.py            # Backend logic (LSTM, sentiment, scraping)
├── data.csv           # Historical stock price data
├── models/            # Saved LSTM models and scalers
├── requirements.txt   # Required Python libraries
├── .env               # Your Hugging Face API token
└── README.md          # Documentation
```

### ▶️ Step 7: Run the Application
```bash
streamlit run app.py
```
The app will launch automatically in your default browser.

## 💡 Notes
- ✅ Make sure you're using Python 3.8 or higher.
- ✅ Use Google Chrome or Firefox for the best UI experience.
- ⚠️ If newspaper3k fails to scrape some articles, re-run the app—some sources might temporarily block scraping.
- 🧠 The LSTM model auto-trains if not already present in the models/ folder.

## 📄 License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## 📞 Contact
For any inquiries or issues, please reach out to [your-email@example.com](mailto:your-email@example.com).
```
