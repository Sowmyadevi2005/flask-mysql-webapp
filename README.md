
# Flask CRUD Web Application

This is a simple **Flask-based web application** that performs **CRUD (Create, Read, Update, Delete)** operations using a **MySQL** backend database.

## 🧰 Tech Stack

- **Backend:** Python 3, Flask
- **Database:** MySQL
- **Frontend:** HTML (Jinja2 templating)
- **Deployment Ready:** Can be containerized, deployed on EC2 or behind an ALB

---

## 🚀 Features

- Add new records (Create)
- View all records (Read)
- Update existing entries (Update)
- Delete records (Delete)
- Simple web UI built with Jinja templates

---

## 📦 Project Structure

```
flask-crud-app/
├── app.py                 # Main Flask app
├── templates/             # HTML templates
│   ├── index.html
└── requirements.txt       # Python dependencies
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/flask-mysql-webapp.git
cd flask-crud-app
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

Access it at: `http://localhost:5000`

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
