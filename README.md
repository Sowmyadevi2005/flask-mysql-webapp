
# Simple Flask Web Application

This is a simple **Flask-based web application** that performs **basic operations (Insert and View)** using a **MySQL** backend database.

> 📝 Note: Before inserting records, you must create the required table by visiting the `/create_table` URL in your browser.

---

## 🧰 Tech Stack

- **Backend:** Python 3, Flask
- **Database:** MySQL
- **Frontend:** HTML (Jinja2 templating)
- **Deployment Ready:** Can be containerized, deployed on EC2 or behind an ALB

---

## 🚀 Features

- Add new records (Insert)
- View all records (View)
- Simple web UI built with Jinja templates

> This application does **not support update or delete** operations.

---

## 📦 Project Structure

```
flask-mysql-webapp/
├── app.py                 # Main Flask app
├── templates/             # HTML templates
│   └── index.html
├── config.py              # MySQL configuration
└── requirements.txt       # Python dependencies
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/Sowmyadevi2005/flask-mysql-webapp.git
cd flask-mysql-webapp
```

### 2. Set Up Virtual Environment (optional but recommended)

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure MySQL

Update the `config.py` file with your database credentials:

```python
MYSQL_HOST = 'localhost'
MYSQL_USER = 'youruser'
MYSQL_PASSWORD = 'yourpassword'
MYSQL_DB = 'yourdatabase'
```

### 5. Run the App

```bash
python app.py
```

Access the app at: `http://localhost:5000`

---

### 🔧 Create the Table

Before adding any records, **navigate to**:

```
http://localhost:5000/create_table
```

This will create the required MySQL table automatically.

---

## 🛡️ Security Note

- Always **use environment variables** or a **secrets manager** for production credentials.
- Add **input validation and SQL sanitization** for user data.

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙌 Acknowledgements

- [Flask](https://flask.palletsprojects.com/)
- [MySQL Connector for Python](https://pypi.org/project/mysql-connector-python/)
