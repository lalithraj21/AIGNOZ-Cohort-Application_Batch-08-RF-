# 📌 AIGNOZ Cohort Application – Batch 08 RF

## 📖 Project Overview

This is a full-stack application built as part of the **AIGNOZ Cohort (Batch 08 RF)**.

It consists of:

* ⚛️ Frontend – React.js
* 🟢 Backend – Node.js + Express
* 🤖 ML Service – FastAPI (Python)
* 🗄️ Database – MongoDB

---

## 🚀 Features

* User authentication (JWT-based)
* Email notifications
* ML API integration
* Full-stack architecture (React + Node + FastAPI)
* Secure environment configuration

---

## 🛠️ Tech Stack

| Layer      | Technology       |
| ---------- | ---------------- |
| Frontend   | React.js         |
| Backend    | Node.js, Express |
| ML Service | FastAPI, Python  |
| Database   | MongoDB          |

---

## ⚙️ Setup Instructions

### 🔹 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

---

### 🔹 2️⃣ Setup Frontend

```bash
cd frontend
npm install
```

Run frontend:

```bash
npm run dev
```

---

### 🔹 3️⃣ Setup Backend

```bash
cd backend
npm install
```

### 📄 Create `.env` file in backend

Create a file named `.env` inside the **backend** folder and add:

```env
PORT=5000

MONGO_URI=your_mongodb_connection_string

JWT_SECRET=super_secure_secret_key

ML_API=http://127.0.0.1:8000

EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password
```

### ▶️ Run Backend

```bash
npm run dev
```

---

### 🔹 4️⃣ Setup ML Service (FastAPI)

```bash
cd ml_services
python -m venv venv
```

### Activate virtual environment

**Windows**

```bash
venv\Scripts\activate
```

**Mac/Linux**

```bash
source venv/bin/activate
```

### 📦 Install Requirements

```bash
pip install -r requirements.txt
```

### ▶️ Run ML Service

```bash
uvicorn main:app --reload
```

ML API runs at:

```
http://127.0.0.1:8000
```

---

## 📧 How to Get EMAIL_USER and EMAIL_PASS

To send emails from your app, you need a **Gmail account** and an **App Password**.

### ✅ Step 1: Enable 2-Step Verification

* Go to your Google Account
* Open **Security settings**
* Enable **2-Step Verification**

---

### ✅ Step 2: Generate App Password

* Search: **Google App Passwords**
* Open App Passwords page
* Select:

  * App → Mail
  * Device → Other (Custom Name)
* Click **Generate**

You will get a 16-character password like:

```
abcd efgh ijkl mnop
```

---

### ✅ Step 3: Use in `.env`

```env
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=abcdefghijklmnop
```

⚠️ Important:

* Do NOT use your real Gmail password
* Always use **App Password**

---

## 🧪 Running the Full Project

You need to run **3 services simultaneously**:

| Service    | Command          | Port |
| ---------- | ---------------- | ---- |
| Frontend   | npm run dev      | 3000 |
| Backend    | npm run dev      | 5000 |
| ML Service | uvicorn main:app | 8000 |

---

## 📁 Important Notes

* `node_modules/` is ignored → run `npm install`
* `.env` is ignored → create manually
* `venv/` is ignored → create manually
* Keep secrets safe 🔐

---

## 📌 Future Improvements

* Deployment (Render / AWS)
* Better UI/UX
* Advanced ML models
* Email templates

---
