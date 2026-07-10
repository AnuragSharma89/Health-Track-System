
# 🏥 Health Track System

**B.Tech CSE Final Year Project — Techno Bengal Institute of Technology (MAKAUT)**

A comprehensive, gender-neutral wellness platform for young adults integrating sleep, diet, skincare, fitness, and mental health tracking into a single dashboard.

---

## 👥 Team

| Name | MAKAUT Roll No. |
|------|----------------|
| Anurag Sharma | 12100122059 |
| Vikash Mahato | 12100122099 |
| Ashu Kr Thakur | 12100122057 |
| Ayush Kumar Sharma | 12100122038 |
| Saurav Kumar Shaw | 12100122098 |

**Mentor:** Prof. Dr. Munshi Mostafijur Rahaman, Dept. of CSE & IT

---

## 📌 Overview

Health Track System is a full-stack wellness platform built with the MERN stack (MongoDB, Express.js, React.js, Node.js). It provides:

- 🛌 Sleep tracking & consistency scoring
- 🥗 Nutrition & hydration logging
- 🏃 Physical activity monitoring
- 🧴 Skincare/dermatological tracking
- 🤒 Rule-based symptom checker
- 📊 Visual analytics dashboard
- 🔐 Secure JWT authentication

Full project documentation, including the formal report, requirement specification, DFDs, and ER diagram, is available in [`/docs`](./docs).

---

## 🏗️ Tech Stack

**Frontend:** React.js · Tailwind CSS · Chart.js · Framer Motion · Axios
**Backend:** Node.js · Express.js · JWT · Bcrypt.js
**Database:** MongoDB + Mongoose ODM
**Deployment:** Vercel/Netlify (frontend) · Render/Railway (backend) · MongoDB Atlas (DB)

---

## 📁 Project Structure

```
health-track-system/
├── frontend/          # React client
├── backend/           # Express API
├── docs/              # Project report, DFDs, ER diagram
└── README.md
```

---

## 🚀 Getting Started

### Prerequisites
- Node.js >= 18.x
- MongoDB (local or Atlas)
- npm or yarn

### Installation

```bash
git clone https://github.com/<your-username>/health-track-system.git
cd health-track-system

# Backend
cd backend
npm install

# Frontend
cd ../frontend
npm install
```

### Environment Variables

Copy `.env.example` to `.env` in `/backend` and fill in your own values:

```env
PORT=5000
MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/healthtrack
JWT_SECRET=your_super_secret_key
JWT_EXPIRES_IN=7d
```

### Running the App

```bash
# Backend (from /backend)
npm run dev

# Frontend (from /frontend)
npm run dev
```

App runs at `http://localhost:5173` (frontend) and `http://localhost:5000` (backend API).

---

## 🔑 Core Algorithms

**Habit Consistency Score**
```
Consistency Score = Σ(Weight × Adherence) ÷ Σ(Weights)
```

**Rule-Based Symptom Mapping** — maps reported symptom clusters to predefined wellness guidance.

**Time-Series Trend Analysis** — tracks sleep, nutrition, mood, and stress over time to detect patterns.

---

## 📊 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register` | Register new user |
| POST | `/api/auth/login` | Login & get JWT |
| GET | `/api/health/dashboard` | Get dashboard stats |
| POST | `/api/health/sleep` | Log sleep entry |
| POST | `/api/health/nutrition` | Log meal entry |
| POST | `/api/health/symptoms` | Log symptoms |
| GET | `/api/health/insights` | Get analytics & trends |

---

## 🔐 Security

- JWT-based stateless authentication
- Bcrypt.js password hashing (salt rounds: 12)
- Input validation & sanitization on all endpoints
- HTTPS enforced in production

---

## 📚 References

1. Smith & Kumar (2020) — Mobile Health Applications: Trends and Prospects
2. World Health Organization (2021) — Global Digital Health Strategy
3. Patel et al. (2019) — Adoption of Wellness Apps Among University Students
4. Johnson & Lee (2022) — Impact of Lifestyle Tracking
5. Statista (2023) — Global mHealth Usage Statistics

---

## 📄 License

This project is developed for academic purposes under MAKAUT, B.Tech CSE curriculum.
