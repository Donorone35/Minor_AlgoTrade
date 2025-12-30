# AlgoTrade - Algorithmic Trading Platform

![AlgoTrade](https://github.com/user-attachments/assets/f4da8ade-591f-4aa4-aeb8-57c52db5fa26)


## 📌 Overview
AlgoTrade is an advanced algorithmic trading platform designed to assist traders in making data-driven decisions. The platform leverages machine learning models to provide intelligent trade recommendations and integrates with market data APIs to fetch real-time information, helping users execute trades based on quantitative analysis rather than emotions.

Link - https://project-mocha-delta-69.vercel.app/

## 🚀 Features
- 📈 **Real-Time Market Data**: Integration with Polygon.io API for historical and real-time stock data
- 🤖 **ML-Based Predictions**: Multiple prediction models including Momentum Moving Average, MACD, Sentiment Analysis, and Time Series Windowing
- 🔄 **Auto Trading System**: Configure and execute automated trading based on model signals
- 📊 **Interactive Dashboard**: Visual representation of market trends and trading performance
- 🛡️ **Risk Management**: Built-in stop-loss and take-profit features to protect investments
- 🎯 **Responsive UI**: Modern interface built with React and Tailwind CSS

## 🛠️ Tech Stack
### **Frontend**
- **React** (built with Vite)
- **Tailwind CSS** for styling
- **Framer Motion** for animations

### **Backend**
- **Node.js** + **Express.js** for Stock Data API
- **Python** for Machine Learning models

### **Data & APIs**
- **Polygon.io API** for stock market data
- **CSV & JSON** for data storage and exchange

## 🔐 Environment Variables & API Keys
The application uses environment variables to secure sensitive data:

1. Create a `.env` file in the root directory
2. Add your Polygon.io API key:
```
POLYGON_API_KEY=your_polygon_api_key_here
```

⚠️ **IMPORTANT**: 
- Never commit your `.env` file to Git (it's already added to `.gitignore`)
- Set environment variables through your hosting platform when deploying
- For development teams, use a `.env.example` file with empty placeholders

## 🏗️ Project Structure
```
AlgoTrade/
│── data/                # Stock data storage
│── models/              # Machine learning model files
│── public/              # Static assets
│── src/                 # Frontend source code
│   │── assets/          # Images and resources
│   │── components/      # React components
│   │── App.jsx          # Main React component
│   │── index.css        # Global styles
│   │── main.jsx         # React entry point
│── server.js            # Express.js backend for stock data
│── server.py            # Python server for ML predictions
│── .env                 # Environment variables (not in Git)
│── requirements.txt     # Python dependencies
│── package.json         # Node.js dependencies
│── vite.config.js       # Vite configuration
│── tailwind.config.js   # Tailwind CSS configuration
```

## 🖥️ Installation & Setup
Follow these steps to set up the complete application:

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/your-username/AlgoTrade.git
cd AlgoTrade
```

### **2️⃣ Set Up Environment Variables**
```bash
# Create and edit .env file with your API key
echo "POLYGON_API_KEY=your_polygon_api_key_here" > .env
```

### **3️⃣ Install Dependencies**
```bash
# Node.js dependencies
npm install

# Python dependencies
pip install -r requirements.txt
```

### **4️⃣ Launch the Application (3 separate terminals)**
**Terminal 1: Stock Data Server (Node.js)**
```bash
node server.js
# Server will run on http://localhost:5000
```

**Terminal 2: ML Prediction Server (Python)**
```bash
python server.py
# Server will run on http://localhost:5001
```

**Terminal 3: Frontend (React)**
```bash
npm run dev
# Application will run on http://localhost:5173
```

### **5️⃣ Access the Application**
Open your browser and navigate to `http://localhost:5173`

## 📌 Running Services & Ports
| Service              | Port  | Description                          |
|----------------------|-------|--------------------------------------|
| Frontend (Vite)      | 5173  | React user interface                 |
| Backend (Express)    | 5000  | Stock data API                       |
| ML Server (Python)   | 5001  | ML prediction models                 |

## 📌 API Endpoints

### Stock Data API (Node.js - Port 5000)
| Method | Endpoint          | Description                      |
|--------|-------------------|----------------------------------|
| GET    | `/api/check-file` | Check if stock data file exists  |
| GET    | `/api/fetch-data` | Fetch and save fresh stock data  |

### ML Prediction API (Python - Port 5001)
| Method | Endpoint                    | Description                      |
|--------|----------------------------|----------------------------------|
| GET    | `/api/check-file`          | Check if stock data exists       |
| GET    | `/api/fetch-data`          | Fetch and save fresh stock data  |
| GET    | `/api/predict`             | Predict using Moving Average     |
| GET    | `/api/predict-sentiment`   | Predict using Sentiment Analysis |
| GET    | `/api/predict-momentum`    | Predict using Momentum strategy  |
| GET    | `/api/predict-macd`        | Predict using MACD indicators    |
| GET    | `/api/predict-transformer` | Predict using Transformer model  |

## 🔍 Troubleshooting
- **API Key Error**: Verify your Polygon API key is correctly set in `.env`
- **Missing Data**: Use the `/api/fetch-data` endpoint to download fresh data
- **Connection Issues**: Ensure all three servers are running simultaneously
- **CORS Problems**: All servers are configured for localhost development by default
- **Model Errors**: Check Python console for detailed ML model error messages

## 📊 Demo Screenshots
<img width="959" alt="image" src="https://github.com/user-attachments/assets/e85f5b1b-7128-4e32-b331-44e990f57d0f" />
<img width="959" alt="image" src="https://github.com/user-attachments/assets/9d22103e-9055-478c-8165-93c3e1254e84" />



## 📬 Contact
- 🐙 GitHub: [Rishabh-tesla-arc](https://github.com/Rishabh-tesla-arc)
- 🔗 LinkedIn: [Rishabh Shrivastav](https://www.linkedin.com/in/rishabhshrivastav-swe/)

---
**⭐ If you like this project, give it a star!** 🚀

