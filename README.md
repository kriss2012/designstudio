# 🎨 DesignStudio – Smart Project & Service Platform

## 👨‍💻 Developed by Krishna Patil  
AI Engineer | Full Stack Developer | Computational Science Student  
📍 Pachora, Maharashtra, India  
📧 202krishnapatil@gmail.com  
🔗 GitHub: https://github.com/kriss2012  

---

## 🌐 Live Demo https://designstudio-k1yc.onrender.com

🚀 Deploy on Render / Railway / Heroku  
(Replace with your deployed URL once live)

Example:
https://your-designstudio-app.onrender.com

---

## 📌 About DesignStudio

**DesignStudio** is a full-stack Flask-based platform that allows users to:

- Purchase custom development projects  
- Request maintenance services  
- Submit contact inquiries  
- Make secure online payments  
- Login securely using Google OAuth  

It includes an Admin Dashboard to monitor users, orders, and maintenance requests.

---

## 🚀 Features

### 🔐 Authentication
- Google OAuth 2.0 Login
- Secure session management
- Role-based access (Admin/User)

### 💳 Razorpay Payment Integration
- Dynamic order creation
- Secure payment verification
- Order status tracking
- Email confirmations

### 🛠 Maintenance Request System
- Submit issue details
- Add optional services
- Cost estimation
- Status tracking

### 📬 Contact API
- Customer inquiry form
- Stores queries in database
- Email notification to admin

### 👑 Admin Dashboard
- View all users
- Track orders
- Monitor revenue
- View maintenance requests

### 📧 Email Automation
- Payment confirmation
- Admin alerts
- Maintenance confirmation

---

## 🛠 Tech Stack

### Backend
- Python
- Flask
- SQLAlchemy
- SQLite (Local) / PostgreSQL (Production)

### Frontend
- HTML5
- CSS3
- JavaScript

### Authentication
- Google OAuth 2.0
- Authlib

### Payments
- Razorpay API

### Email Service
- SMTP (Gmail)

---

## ⚙️ Installation Guide (Local Setup)

### 1️⃣ Clone Repository

```bash
git clone https://github.com/kriss2012/designstudio.git
cd designstudio
````

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

Activate:

**Windows**

```bash
venv\Scripts\activate
```

**Mac/Linux**

```bash
source venv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install flask flask_sqlalchemy authlib razorpay python-dotenv
```

Or if using requirements.txt:

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables Setup

Create a `.env` file in the root directory:

```env
# --- GENERAL ---
SECRET_KEY=your_secret_key

# --- GOOGLE OAUTH ---
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret

# --- RAZORPAY ---
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret

# --- EMAIL ---
MAIL_USERNAME=your_email@gmail.com
MAIL_PASSWORD=your_email_password
```

⚠ For Gmail:
Use App Password instead of your real password.

---

## ▶ Run the Application

```bash
python app.py
```

Open browser:

```
http://127.0.0.1:5000
```

---

## 📂 Project Structure

```
/designstudio
│
├── app.py
├── studio.db
├── .env
│
├── templates/
│   └── index.html
│
├── static/
│   ├── style.css
│   └── script.js
│
└── README.md
```

---

## 🔐 API Endpoints

| Endpoint           | Method | Description                |
| ------------------ | ------ | -------------------------- |
| `/login`           | GET    | Google OAuth login         |
| `/logout`          | GET    | Logout user                |
| `/create_order`    | POST   | Create Razorpay order      |
| `/payment_success` | POST   | Confirm payment            |
| `/api/contact`     | POST   | Submit contact form        |
| `/api/maintenance` | POST   | Submit maintenance request |
| `/api/my_orders`   | GET    | Get user orders            |
| `/api/admin/data`  | GET    | Admin analytics            |

---

## ☁ Deployment (Render Example)

1. Push code to GitHub
2. Go to [https://render.com](https://render.com)
3. Create New → Web Service
4. Connect repository

### Settings:

Build Command:

```bash
pip install -r requirements.txt
```

Start Command:

```bash
gunicorn app:app
```

Add all environment variables in Render dashboard.

Update Google OAuth redirect URI:

```
https://your-app-name.onrender.com/authorize
```

---

## 🛡 Security Highlights

* OAuth 2.0 authentication
* Secure payment verification
* Environment-based secret management
* Admin access restriction

---

## 📊 Future Improvements

* User dashboard UI
* Order tracking page
* Payment history export
* Role-based admin panel
* Email templates upgrade
* Stripe integration option

---

## ❤️ Credits

Developed by:

**Krishna Patil**
AI Engineer | Full Stack Developer
Computational Science Student

📧 [202krishnapatil@gmail.com](mailto:202krishnapatil@gmail.com)
🔗 [https://github.com/kriss2012](https://github.com/kriss2012)

---

## 📜 License

MIT License © 2026 Krishna Patil

```