# 🍓 Fruitable — E-Commerce Web Application
 
A fully functional e-commerce website for a fruit store, developed as an internship project. Built with **Python Flask**, **MySQL**, and **HTML/CSS**, featuring user authentication, role-based access control, and a dedicated admin panel.
 
---
 
## 📌 Project Overview
 
Fruitable is a multi-page e-commerce platform that allows customers to browse and purchase fruits online. The application supports secure user registration and login, a smooth shopping experience across multiple pages, and a powerful admin panel for managing users, products, and site-wide data.
 
---
 
## 🚀 Features
 
### 👤 User Side
- **Authentication System** — Secure Login and Registration with session-based redirection to the home page upon successful login
- **Multi-Page Navigation** — Home, Customer, Purchase, Contact, and Profile sections for a seamless shopping experience
- **Purchase Management** — Users can browse products and complete purchases
 
### 🔐 Admin Panel
- Separate admin login with elevated privileges
- Access to all registered user information and login activity
- Full site-wide data management at any time
 
### 🗄️ Database & Backend
- MySQL database managed via **WAMP Server** to handle user records, product data, and purchase information
- **Python Flask** backend for routing, form processing, and server-side logic
 
---
 
## 🛠️ Tech Stack
 
| Layer      | Technology              |
|------------|-------------------------|
| Frontend   | HTML, CSS               |
| Backend    | Python (Flask)          |
| Database   | MySQL                   |
| Server     | WAMP Server             |
 
---
 
## 📁 Project Structure
 
```
fruitable/
│
├── static/
│   └── img/                    # Images and assets
│
├── templates/
│   ├── css/                    # Stylesheets
│   ├── js/                     # JavaScript files
│   ├── lib/                    # Frontend libraries
│   ├── scss/                   # SCSS source files
│   │
│   ├── index.html              # Home page
│   ├── loginform.html          # User login
│   ├── registerform.html       # User registration
│   ├── customer.html           # Customer section
│   ├── showcart.html           # Shopping cart
│   ├── userprofile.html        # User profile
│   ├── contact.html            # Contact page
│   ├── admin.html              # Admin panel
│   ├── welcomeadmin.html       # Admin dashboard
│   ├── PrivacyPolicy.html      # Privacy policy
│   ├── salesrefunds.html       # Sales & refunds policy
│   ├── termsuser.html          # Terms of use
│   └── samplecon.html          # Sample content page
│
├── ar_master.py                # Main Flask application
└── main.py                     # App entry point
```
 
---
 
## ⚙️ Setup & Installation
 
### Prerequisites
- Python 3.x
- WAMP Server (MySQL + Apache)
- pip
 
### Steps
 
1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/fruitable.git
   cd fruitable
   ```
 
2. **Install Python dependencies**
   ```bash
   pip install -r requirements.txt
   ```
 
3. **Set up the database**
   - Start WAMP Server and ensure MySQL is running
   - Create a new database named `fruitable_db`
   - Import the provided SQL schema:
     ```bash
     mysql -u root -p fruitable_db < database/schema.sql
     ```
 
4. **Configure the application**
   - Update `config.py` with your MySQL credentials:
     ```python
     DB_HOST = 'localhost'
     DB_USER = 'root'
     DB_PASSWORD = 'your_password'
     DB_NAME = 'fruitable_db'
     ```
 
5. **Run the Flask application**
   ```bash
   python main.py
   ```
   > The core application logic lives in `ar_master.py`, loaded via `main.py`.
 
6. **Open in your browser**
   ```
   http://localhost:5000
   ```
 
---
 
## 🔑 Admin Access
 
To access the Admin Panel, navigate to:
```
http://localhost:5000/admin/login
```
Use the admin credentials configured in your database.
 
---
 
## 📸 Screenshots
 
> *(Add screenshots of the Home page, Login page, and Admin Dashboard here)*
 
---
 
## 🙌 Acknowledgements
 
- Developed as part of an **internship project**
- HTML templates were customized and adapted for the Fruitable brand
- Special thanks to the internship organization for guidance and support
 
---
 
## 📄 License
 
This project is for educational and internship purposes. All rights reserved.
