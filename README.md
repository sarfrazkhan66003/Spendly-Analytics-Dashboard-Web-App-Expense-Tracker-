# 💰 Spendly — Smart Expense Tracker Web App

Spendly is a **Flask-based Expense Tracking Web Application** designed to help users **track daily expenses, analyze spending patterns, and manage finances effectively**.

Inspired by modern finance tools, Spendly provides a clean dashboard, category-based tracking, and analytics to give users complete financial visibility. ([Spendly][1])

---

## 🚀 Why This Project is Important?

Managing personal finances is a common problem:

* ❌ People don’t know where money goes
* ❌ No structured tracking system
* ❌ Difficult to analyze spending patterns

👉 Spendly solves this by:

* Providing **category-based expense tracking**
* Offering **analytics & summaries**
* Helping users build **financial discipline**

---

## 🎯 Key Features

* 🔐 User Authentication (Login & Register)
* 💸 Add Expenses with Categories
* 📊 Dashboard with Summary Stats
* 📅 Date-wise Filtering (Monthly / Custom)
* 📂 Category-wise Breakdown
* 🧾 Recent Transactions History
* 🔒 Secure Password Handling
* 📈 Analytics Page (UI Ready)

---

## 🛠️ Tech Stack

| Layer        | Technology                  |
| ------------ | --------------------------- |
| Backend      | Flask (Python)              |
| Frontend     | HTML, CSS, Jinja Templates  |
| Database     | SQLite                      |
| Auth         | Werkzeug Security           |
| Architecture | MVC (Model-View-Controller) |

---

## 🧠 System Architecture

```bash
User → Flask Routes → Business Logic → SQLite DB → Response (HTML Templates)
```

---

## 📂 Project Structure

```bash
Spendly/
│── app.py                # Main Flask Application
│── database/
│   ├── db.py            # DB Connection & Setup
│   ├── queries.py       # SQL Queries
│── templates/           # HTML Pages
│── static/              # CSS, JS, Assets
│── tests/               # Unit Tests
│── requirements.txt
│── spendly.db           # SQLite Database
```

---

## ⚙️ Python Version

```bash
Python 3.8+
```

👉 Recommended:

```bash
Python 3.10 or 3.11
```

---

## ⚙️ How It Works (Workflow)

### 1️⃣ User Registration

* User enters name, email, password
* Password is securely hashed
* Stored in SQLite database

### 2️⃣ User Login

* Credentials verified using hashed password
* Session is created

### 3️⃣ Add Expense

* User inputs:

  * Amount
  * Category
  * Date
  * Description
* Data validated and stored

### 4️⃣ Dashboard Processing

System calculates:

* Total spending
* Category breakdown
* Recent transactions
* Date-based filtering

---

## 🧮 Core Algorithm Logic

### Expense Filtering Algorithm

```python
if date_from and date_to:
    filter expenses between date range
else:
    show all expenses
```

### Summary Calculation

```python
total = sum(all expenses)
category_total = group by category
recent_transactions = latest entries
```

### Date Handling

* Custom `_parse_date()` ensures valid input
* `_months_ago()` calculates past date ranges

---

## 📸 Screenshots Explanation

### 🏠 Landing Page

<img width="1915" height="1031" alt="Screenshot 2026-05-03 012840" src="https://github.com/user-attachments/assets/4cfb7454-75fd-4743-a696-8f90e15904aa" />

* Introduction to Spendly
* Call-to-action (Login / Register)

### 🔐 Login Page
<img width="1919" height="938" alt="Screenshot 2026-05-03 012904" src="https://github.com/user-attachments/assets/62336258-829a-4fa5-afb8-fe5976feb3dd" />

* Secure authentication form
* Error handling for invalid credentials

### 📝 Register Page
<img width="1919" height="933" alt="Screenshot 2026-05-03 012852" src="https://github.com/user-attachments/assets/588c132f-b1da-4d27-9422-06fe38eabf8a" />

* User account creation
* Password validation

### 📊 Dashboard (Profile Page)

* Total expenses summary
* Category-wise breakdown
* Recent transactions
* Date filters

---

## 🔄 Installation & Setup

### 1️⃣ Clone Repository

```bash
git clone [https://github.com/YOUR_USERNAME/Spendly-Expense-Tracker-Flask.git](https://github.com/sarfrazkhan66003/Spendly-Analytics-Dashboard-Web-App-Expense-Tracker-/new/main?filename=README.md)
cd Spendly-Expense-Tracker-Flask
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Run Application

```bash
python app.py
```

### 5️⃣ Open Browser

```bash
http://127.0.0.1:5001/
```

---

## 🧪 Testing

```bash
pytest
```

---

## 📈 Future Enhancements

* 🤖 AI-based expense prediction
* 📊 Advanced charts (Power BI / Chart.js)
* ☁️ Cloud database (PostgreSQL)
* 📱 Mobile responsive UI
* 🔔 Budget alerts

---

## 🎯 Use Cases

* Students tracking expenses
* Personal finance management
* Budget planning

---

## 🤝 Contributing

1. Fork the repo
2. Create a new branch
3. Commit your changes
4. Push and create PR

---

## 📜 License

MIT License

---

## 👨‍💻 Author

**Sarfraz Khan**
B.Tech AI & Data Science
Aspiring Data Scientist 🚀
