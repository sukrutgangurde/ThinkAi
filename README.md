# ThinkAI 🤖💬

ThinkAI is a **full-stack ChatGPT-like AI application** built using **React (Vite)** for the frontend and **Node.js + Express + MongoDB** for the backend. It uses **OpenAI GPT-4.0 Mini** to generate intelligent responses and supports **multiple chat threads** stored in MongoDB.

---

## 🚀 Features

* ChatGPT-style AI chat interface
* GPT-4.0 Mini integration
* Multiple chat threads (conversation history)
* MongoDB for persistent storage
* Syntax-highlighted AI responses (code support)
* Modern dark UI

---

## 🛠 Tech Stack

### Frontend

* React (Vite)
* Context API
* React Markdown + Highlight.js

### Backend

* Node.js
* Express.js
* MongoDB (Atlas)
* OpenAI API (GPT-4.0 Mini)

---

## 📦 Project Structure

```
ThinkAI/
│
├── Backend/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   ├── server.js
│   ├── package.json
│   └── .env (not committed)
│
├── Frontend/
│   ├── src/
│   ├── public/
│   ├── index.html
│   ├── vite.config.js
│   └── package.json
│
└── .gitignore
```

---

## ⚙️ Setup & Run Locally

Follow these steps carefully to run the project on your local machine.

---

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/sukrutgangurde/ThinkAi.git
cd ThinkAi
```

---

### 2️⃣ Backend Setup

#### Install dependencies

```bash
cd Backend
npm install
```

#### Create `.env` file inside `Backend/`

```env
OPENAI_API_KEY=your_openai_api_key
MONGODB_URI=your_mongodb_cluster_url
PORT=8080
```

> ⚠️ **Never commit `.env` files**. They are already ignored via `.gitignore`.

---

### 3️⃣ Create OpenAI ChatGPT API Key

* Go to **OpenAI Dashboard**
* Create an API key
* Make sure your account has access to **GPT-4.0 Mini**
* Paste the key into `OPENAI_API_KEY` in `.env`

---

### 4️⃣ Create MongoDB Cluster

* Go to **MongoDB Atlas**
* Create a free cluster
* Get the connection string
* Paste it into `MONGODB_URI` in `.env`

---

### 5️⃣ Run Backend Server

```bash
npm run dev
```

OR

```bash
nodemon server.js
```

Backend will start on:

```
http://localhost:8080
```

---

### 6️⃣ Frontend Setup

Open a **new terminal** and run:

```bash
cd Frontend
npm install
npm run dev
```

Frontend will start on:

```
http://localhost:5173
```

---

## ✅ How It Works

1. User sends a message from the frontend
2. Request goes to Express backend
3. Backend calls **GPT-4.0 Mini** via OpenAI API
4. Response is stored in MongoDB
5. Conversation history is rendered in UI

---

## 🔒 Security

* API keys stored safely in `.env`
* `.env` and `node_modules` are ignored
* No sensitive data pushed to GitHub

---

## 📌 Future Improvements

* Authentication (Login / Signup)
* Streaming AI responses
* Light/Dark theme toggle
* Deployment (Vercel + Render)

---

## ❤️ Author

**Sukrut Gangurde**
Built with passion & curiosity.

---

⭐ If you like this project, give it a star!
