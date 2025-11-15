# 🩺 Real-Time Patient Queue Management System

A modern, scalable, and real-time digital solution to replace physical queues in hospitals, clinics, and any service centers — built using **Django REST Framework**, **React Native**, **React.js**, and **WebSockets**.

---

## 🚀 Overview

Patients often wait for hours in hospitals without knowing their actual turn. This leads to:

* Stress & discomfort
* Overcrowding
* Repeated inquiries at reception
* Bad patient experience

This project solves the problem using a **real-time queue tracking system** where:

* Patients register remotely using a mobile app
* Doctors manage the queue through a dashboard
* Everyone receives real-time token updates

---

## 📸 Demo Screenshots

> 🔽 Add your app/dashboard images here after uploading.

---

## 🏗️ Architecture

**1. Patient Mobile App (React Native)**

* Remote registration
* Live token & ETA tracking

**2. Doctor Dashboard (React.js)**

* Queue control (Next, Skip, Complete)
* Real-time patient list updates

**3. Backend (Django REST Framework)**

* Authentication (Patients + Doctors)
* Queue & token management logic
* Notification handling

**4. Real-Time Layer**

* WebSockets / Push Notifications

**5. Database**

* PostgreSQL / SQLite3

---

## 🔧 Tech Stack

### **Frontend**

* React Native (Patient App)
* React.js (Doctor Dashboard)

### **Backend**

* Python, Django REST Framework
* Django Channels (for real-time updates)

### **Database**

* PostgreSQL / SQLite3

### **Notifications**

* Push / SMS support (optional)

---

## ⭐ Features

* ✔ Remote patient registration
* ✔ Real-time token number & ETA
* ✔ Multi-doctor / multi-clinic support
* ✔ Admin dashboard with crowd heatmap
* ✔ Accessibility mode for seniors
* ✔ Push/SMS reminders

---

## 🛠️ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/sanij0579/Doctor-patient-Queue-app.git
cd Doctor-patient-Queue-app
```

### 2️⃣ Backend Setup (Django)

```bash
cd backend
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Backend will run at:

```
http://127.0.0.1:8000/
```

### 3️⃣ Mobile App Setup (React Native)

```bash
cd mobile-app
npm install
npm start
```

Use Expo Go or emulator to run the app.

### 4️⃣ Doctor Dashboard Setup (React.js)

```bash
cd doctor-dashboard
npm install
npm start
```

Dashboard runs at:

```
http://localhost:3000/
```

---

## 📡 API Overview

### Authentication

* `/api/register/` – Register patient
* `/api/login/` – Login
* `/api/doctor/login/` – Doctor login

### Queue Management

* `/api/queue/join/` – Take token
* `/api/queue/current/` – Get current token
* `/api/queue/next/` – Doctor proceeds next
* `/api/queue/skip/` – Skip patient

---

## 📂 Folder Structure (Recommended)

```
Doctor-patient-Queue-app/
│
├── backend/                # Django backend
├── mobile-app/             # React Native App
├── doctor-dashboard/       # React.js Dashboard
├── README.md               # Project documentation
└── LICENSE
```

---

## 📊 Expected Impact

* ⬇ 40% reduction in physical waiting time
* ⬇ 25% fewer reception inquiries
* ⭐ Better patient experience
* 📉 Reduced crowding
* 🏥 Smooth hospital operations

---

## 🔭 Future Enhancements

* AI-based wait time prediction
* Voice announcements in local languages
* Integration with EMR/Hospital systems
* Role-based permissions
* Predictive analytics for crowd management

---

## 🤝 Contributing

Contributions are welcome! Feel free to open issues and pull requests.

---

## 📝 License

This project is open-source and available under the **MIT License**.

---

## 🎯 Goal

**To make healthcare faster, smarter, and more patient-friendly — one queue at a time.**
