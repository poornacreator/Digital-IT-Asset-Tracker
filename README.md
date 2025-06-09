# 🖥️ Digital IT Asset Tracker

**A Flask-based IT Asset Management System** to track and manage IT assets efficiently, including purchase dates, warranty status, and user assignments.

## 📌 Features
✅ **User Authentication** (Secure Login & Registration)  
✅ **Asset Management** (Add, View, Update, Delete)  
✅ **Database Storage** (SQLite-based persistent storage)  
✅ **REST API Endpoints** (Integration-ready for other systems)  
✅ **User Assignment System** (Track assets per employee)  

## 🚀 Installation & Setup

### **Prerequisites**
Ensure you have the following installed:
- Python 3.8+
- Flask (`pip install flask`)
- SQLite (Pre-installed with Python)

### **Setup Instructions**
```bash
git clone https://github.com/your-repo/IT-Asset-Tracker.git
cd IT-Asset-Tracker
pip install flask
python app.py

##📌 The server will start at http://127.0.0.1:5000


Endpoint	Method	Description
/register	POST	User registration
/login	POST	User authentication
/assets	GET	Retrieve all assets
/assets	POST	Add a new asset
/assets/<id>	PUT	Update an asset
/assets/<id>	DELETE	Delete an asset

##💡 Usage Example

Register a User

curl -X POST http://127.0.0.1:5000/register -H "Content-Type: application/json" \
-d '{"username": "admin", "password": "securepass"}'

Add an IT Asset

curl -X POST http://127.0.0.1:5000/assets -H "Content-Type: application/json" \
-d '{"name": "Laptop", "category": "Electronics", "purchase_date": "2025-06-10", "warranty": "2 years", "assigned_to": "John Doe"}'

Retrieve All Assets

curl -X GET http://127.0.0.1:5000/assets

🛠️ Future Enhancements
🔹 Email Notifications for asset warranty expiry 🔹 Interactive Web Dashboard for visualizing asset usage 🔹 Role-Based Access Control for multi-user functionality

🤝 Contributing
Feel free to fork the repository and submit pull requests. For major changes, open an issue first.
