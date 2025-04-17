# AI-Based Stock Market Investment Advisor 📈🤖

*Empowering retail investors with AI-driven insights*

---

## 📌 Overview
An AI-powered stock prediction system that forecasts NSE stock prices using LSTM neural networks. Features a Tkinter GUI for real-time visualizations, portfolio recommendations, and secure user management via MySQL.

**Developed By**:  
Tharun A | Svaraan Kumar Thammu | Surya Narayanan S  
**Supervisor**: Mr. Aravindan M  
**Department**: Electronics and Communication Engineering, SRM Institute of Science and Technology  

---

## 🚀 Key Features
- **Real-Time Data**: Fetches NSE stock data using `yfinance` (TCS.NS, RELIANCE.NS, INFY.NS etc.)
- **AI Predictions**: Dual-layer LSTM model for 10-day price forecasts (RMSE: 2.34, MAE: 1.89)
- **Portfolio Recommendations**: Risk-return analysis with probability scoring
- **Interactive Dashboard**: 
  - Single stock prediction graphs
  - Investment amount calculator
  - Historical performance tracking
- **Secure Authentication**: MySQL-backed user accounts with prediction history

---

## 🛠️ Installation Guide

### Prerequisites
- Python 3.8+
- MySQL Server 8.0+
- 4GB RAM (minimum)

## Features
- User authentication system
- Single stock price prediction
- Investment recommendations
- Prediction history tracking
- Interactive visualizations

## Installation
```bash
# Install dependencies
pip install -r requirements.txt

# Setup MySQL database
mysql -u root -p < database_schema.sql

# Update database credentials in db.py

### Step-by-Step Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/1sanemax/stock-prediction-system.git
   cd stock-prediction-system

2. **Update credentials in db.py:**
   ```bash
    connection = mysql.connector.connect(
        host="localhost",
        user="your_username",
        password="your_password",
        database="stock_prediction"
    )

3. **Usage**
   ```bash
   python interface.py
```
---
## 🖥️ User Manual
### Login Screen
  -New users can register with email/password

  -Existing users login to access dashboard

### Dashboard Features:
#### 1.Single Stock Prediction:

  -Select from 5 NSE stocks
    
  -View 10-day price forecast with historical comparison

#### 2.Portfolio Advisor:

  -Enter investment amount (₹1,000 - ₹1,00,000)

  -Set time horizon (7-90 days)

  -Get AI-ranked stock recommendations

#### 3.Prediction History:

  -Track all previous forecasts

  -Filter by date/stock/profitability

## 🏗️ System Architecture
### Technical Stack:
  -Frontend: Tkinter, Matplotlib

  -Backend: Python 3.8, TensorFlow 2.13
  
  -Database: MySQL 8.0
  
  -Data Sources: yFinance API
