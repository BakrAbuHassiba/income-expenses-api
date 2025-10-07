#  Income & Expenses API

A RESTful backend API to manage and track user **income** and **expenses** — built to help users organize their financial data efficiently.  
It supports **authentication**, **CRUD operations**, and **secure user-specific data management**.

---



##  Features

- 🔐 User registration & authentication  
- 💵 Manage income and expense records  
- 🧾 CRUD operations (Create, Read, Update, Delete)  
- ⚙️ Input validation & error handling  
- 📊 User-based data separation  
- 🕓 Timestamps for created/updated records  
- (Optional) Filtering, search, and total summaries  

---

## 🧩 Tech Stack

| Component        | Technology / Library                     |
|------------------|-------------------------------------------|
| **Backend**      | Django / Django REST Framework *(or your backend of choice)* |
| **Database**     | SQLite (dev) / PostgreSQL (prod)          |
| **Authentication** | JWT / Token-based auth                 |
| **Environment**  | Python 3.x                                |
| **Deployment**   | (Heroku / Docker / Render — optional)     |

---

## 🚀 Getting Started

### Prerequisites

Before running, ensure you have:

- Python 3.x installed  
- `pip` (Python package manager)  
- Virtual environment tool (`venv`, `virtualenv`, etc.)

---

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/BakrAbuHassiba/income-expenses-api.git
   cd income-expenses-api
   ```
2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   # Activate:
   # Windows:
   venv\Scripts\activate
   ```
3. **Install dependencies**
   pip install -r requirements.txt
### Database & Migrations
4. **Apply migrations**
   python manage.py migrate
5. **(Optional) Create a superuser**
   python manage.py createsuperuser

### Running the Server
6. **Start the development server**
 python manage.py runserver

  ```
| Method | Endpoint              | Description                           |
| ------ | --------------------- | ------------------------------------- |
| POST   | `/api/register/`      | Register a new user                   |
| POST   | `/api/login/`         | Authenticate user and return token    |
| GET    | `/api/incomes/`       | List all income records (user scoped) |
| POST   | `/api/incomes/`       | Create a new income record            |
| GET    | `/api/incomes/<id>/`  | Retrieve a specific income record     |
| PUT    | `/api/incomes/<id>/`  | Update a specific income record       |
| DELETE | `/api/incomes/<id>/`  | Delete a specific income record       |
| GET    | `/api/expenses/`      | List all expense records              |
| POST   | `/api/expenses/`      | Create a new expense record           |
| GET    | `/api/expenses/<id>/` | Retrieve a specific expense record    |
| PUT    | `/api/expenses/<id>/` | Update an expense record              |
| DELETE | `/api/expenses/<id>/` | Delete an expense record              |
```
