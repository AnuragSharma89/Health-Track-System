# 🏥 Health Track System

## 🌐 Live Demo

🚀 **Live Website:** [HealthTrack — Open Website](https://health-track-system.vercel.app)


**B.Tech CSE Project — Techno Bengal Institute of Technology**

A comprehensive, gender-neutral wellness platform for young adults integrating sleep, nutrition, skincare, fitness, and mental health tracking.

## 👥 Team

| Name | MAKAUT Roll No. |
|---|---|
| Anurag Sharma | 12100122059 |
| Vikash Mahato | 12100122099 |
| Ashu Kr Thakur | 12100122057 |
| Ayush Kumar Sharma | 12100122038 |
| Saurav Kumar Shaw | 12100122098 |

**Mentor:** Prof. Dr. Munshi Mostafijur Rahaman, Department of CSE & IT

## 📌 Project Overview

Health Track System is a full-stack wellness platform built with React.js, Node.js, Express.js, and MongoDB. It provides:

- 🛌 Sleep tracking and consistency scoring
- 🥗 Nutrition and hydration logging
- 🏃 Physical activity monitoring
- 🧴 Skincare tracking
- 🤒 Rule-based symptom guidance
- 📊 Visual analytics dashboard
- 🔐 JWT-based authentication

Project documentation, reports, and diagrams are available in the [`docs`](./docs) directory.

## 🏗️ Tech Stack

**Frontend**
- React.js
- Tailwind CSS
- Chart.js
- Framer Motion
- Axios

**Backend**
- Node.js
- Express.js
- JWT authentication
- Bcrypt.js password hashing

**Database**
- MongoDB
- Mongoose ODM

**Deployment options**
- Frontend: Vercel or Netlify
- Backend: Render or Railway
- Database: MongoDB Atlas

## 📁 Project Structure

```text
Final_HealthTrack/
├── frontend/
│   ├── src/
│   ├── index.html
│   └── package.json
├── backend/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── server.js
│   └── package.json
├── docs/
├── .gitignore
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Node.js 18 or later
- npm
- A MongoDB database, such as MongoDB Atlas

### 1. Clone the repository

```bash
git clone https://github.com/AnuragSharma89/Health-Track-System.git
cd Health-Track-System
```

### 2. Install backend dependencies

```bash
cd backend
npm install
```

### 3. Configure environment variables

Create a file named `.env` inside the `backend` directory.

Add your own configuration:

```dotenv
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_random_secret
JWT_EXPIRES_IN=7d
GEMINI_API_KEY=your_gemini_api_key
```

Use the Gemini API key only if you want to enable the AI Assistant. Do not commit `.env` or share your credentials publicly.

### 4. Start the backend

From the `backend` directory, run:

```bash
npm run dev
```

The backend API runs at:

`http://localhost:5000/api`

### 5. Install frontend dependencies

Open a second terminal from the project root:

```bash
cd frontend
npm install
```

### 6. Start the frontend

```bash
npm run dev
```

Open the local URL printed by Vite in your terminal. It may use port `5173` or another available port.

## 🔑 Core Algorithms

**Habit Consistency Score**

Calculates consistency using weighted adherence:

```text
Consistency Score = Σ(Weight × Adherence) / Σ(Weights)
```

**Rule-Based Symptom Mapping**

Matches user-reported symptom patterns against predefined rules to provide wellness guidance. It is not a substitute for professional medical advice.

**Time-Series Trend Analysis**

Tracks wellness metrics such as sleep, nutrition, mood, and stress over time to help identify patterns.

## 📊 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/auth/register` | Register a user |
| POST | `/api/auth/login` | Authenticate a user |
| GET | `/api/health/dashboard` | Retrieve dashboard statistics |
| POST | `/api/health/sleep` | Record sleep data |
| POST | `/api/health/nutrition` | Record nutrition data |
| POST | `/api/health/symptoms` | Record symptoms |
| GET | `/api/health/insights` | Retrieve analytics and trends |

Availability of individual endpoints depends on the backend implementation.

## 🔐 Security

- JWT-based authentication
- Bcrypt password hashing
- Environment variables for secrets and configuration
- Input validation and sanitization where implemented
- HTTPS for production deployments

Never commit database credentials, JWT secrets, API keys, or other private configuration.

## 📚 References

1. Smith & Kumar (2020) — Mobile Health Applications: Trends and Prospects
2. World Health Organization (2021) — Global Digital Health Strategy
3. Patel et al. (2019) — Adoption of Wellness Apps Among University Students
4. Johnson & Lee (2022) — Impact of Lifestyle Tracking
5. Statista (2023) — Global mHealth Usage Statistics

## 📄 License

This project was developed for academic purposes as part of the B.Tech CSE curriculum under MAKAUT.
