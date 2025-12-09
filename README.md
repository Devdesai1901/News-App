# 📰 NewsAI — Intelligent News Analysis with LLMs & NLP

**NewsAI** is an AI-powered news intelligence platform that transforms real-time news data into actionable insights using modern NLP and Large Language Models.  
Powered by **Gemini**, **BERT**, **FastAPI**, and **Streamlit**, the system brings together automated news ingestion, sentiment analysis, topic discovery, and interactive visual analytics.


---

## ✨ Overview

NewsAI leverages state-of-the-art AI models and a modular data pipeline to help users:

- Monitor breaking news in real time  
- Analyze sentiment across topics, regions, and time windows  
- Extract summaries, contextual insights, and metadata  
- Visualize news patterns through an interactive Streamlit dashboard  
- Compare historical vs. real-time trends  

---

### ⚙️ Key Features

### 🔮 AI-Powered Insight Engine
- **Gemini LLM** for contextual summaries, keyword extraction, and insight generation  
- **BERT Sentiment Analysis** for polarity classification (positive / neutral / negative)  
- Automated **topic modeling & clustering**  
- Enriched metadata for deeper analytics  

### 📊 Interactive Analytics Dashboard
- Clean, responsive **Streamlit** interface  
- Time-series sentiment trends  
- Topic-level distribution charts  
- Article-level drill-down and summaries  
- Configurable filters (source, topic, date, sentiment)  

### 🚀 Robust & Scalable Backend
- **FastAPI** endpoints with async processing  
- **MongoDB** for flexible article storage  
- Modular ingestion + preprocessing pipeline  
- High-performance design for real-time workloads  

---

### 📦 Tech Stack

| Layer | Technology |
|------|------------|
| **LLM & NLP** | Gemini API, BERT |
| **Backend** | FastAPI, Python |
| **Dashboard** | Streamlit |
| **Database** | MongoDB |
| **Deployment** | Streamlit Cloud |
| **Utilities** | dotenv, pandas, plotly, requests |

---

# 🚀 Quick Start — One-Command Setup Script for NewsAI

### 1️⃣ Clone the repository
git clone https://github.com/Devdesai1901/News-App.git
cd NewsAI

### 2️⃣ Install dependencies
pip install -r requirements.txt

### 3️⃣ Create .env file with required API keys
cat > .env << 'EOF'
NEWS_API_KEY=your_news_api_key
GEMINI_API_KEY=your_gemini_key
MONGO_URI=your_mongo_connection_string
EOF

echo ".env created. Please update it."

### 4️⃣ Run the Streamlit Dashboard
cd src/dashboard
streamlit run app.py


### 5️⃣ (Optional) Run only the processing pipeline
### python -m src.pipeline


## project structure
```bash


NewsAI/
│
├── src/
│   ├── api/              # FastAPI endpoints
│   ├── dashboard/        # Streamlit UI (main dashboard: app.py)
│   ├── models/           # NLP + LLM components (Gemini, BERT, topic models)
│   ├── pipeline.py       # End-to-end ingestion + processing pipeline
│   └── utils/            # Helper scripts (logging, preprocessing, config)
│
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation
└── .env.example           # Template for environment variables


```

