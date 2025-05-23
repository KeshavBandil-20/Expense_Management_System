# 💸 Expense Management Tracker

A full-stack application to track, update, and analyze your daily expenses with a smooth user experience using **Streamlit** for the frontend and **FastAPI** as the backend.

---

## 🚀 Features

- ✅ Add or update daily expenses with category, amount, and notes
- 📊 View analytics and breakdown of expenses over a date range
- 🧠 Smart backend with FastAPI and MySQL
- 🎯 Easy-to-use UI built with Streamlit

---

## 🛠️ Tech Stack

| Layer     | Technology                        |
|-----------|-----------------------------------|
| Frontend  | Streamlit                         |
| Backend   | FastAPI, Pydantic, Uvicorn        |
| Database  | MySQL                             |
| Utilities | Pandas, Pytest                    |

---

## 📂 Folder Structure

├── app.py # Streamlit frontend\
├── server.py # FastAPI backend\
├── db_helper.py # Database operations\
├── requirements.txt # Required packages\
└── README.md # Project documentation\

---
## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/expense-management-system.git
   cd expense-management-system
   ```
1. **Install dependencies:**:   
   ```commandline
    pip install -r requirements.txt
   ```
1. **Run the FastAPI server:**:   
   ```commandline
    uvicorn server.server:app --reload
   ```
1. **Run the Streamlit app:**:   
   ```commandline
    streamlit run frontend/app.py
   ```
 ---  
## 📡 API Endpoints

| Method | Endpoint             | Description                      |
|--------|----------------------|----------------------------------|
| GET    | `/expenses/{date}`   | Retrieve all expenses for a given date |
| POST   | `/expenses/{date}`   | Add or update expenses for a specific date |
| POST   | `/analytics`         | Get expense analytics between two dates |

---
## 📝 Example Input for Analytics Endpoint

```json
{
  "start_date": "2024-08-01",
  "end_date": "2024-08-10"
}
