# Url-shortener-App
# 🔗 URL Shortener with JWT Authentication

A full-stack URL shortener application with secure JWT-based authentication, user-specific analytics, responsive UI, and modular architecture.

---

## 🚀 Features

- **Authentication**: Secure JWT-based login/register  
- **User Management**: Each user manages their own URLs  
- **Analytics Dashboard**: Click tracking with charts and stats  
- **Modern UI**: Component-based React design with clean visuals  
- **Responsive Design**: Fully mobile-friendly  
- **URL Management**: Create, view, delete, and track URLs  
- **Click Analytics**: Real-time performance metrics  
- **Component Architecture**: Scalable and maintainable structure

---

## 🛠️ Tech Stack

- **Backend**: Node.js, Express, MongoDB, JWT  
- **Frontend**: React, TypeScript, Vite  
- **Authentication**: JWT + bcrypt (secure password hashing)  
- **UI Components**: Custom React components with modern CSS

---

## 🧩 Component Overview

### 🔐 AuthForm
- Login/register interface  
- Password visibility toggle  
- Validation feedback

### 🧭 Navbar
- Dynamic navigation bar  
- User profile and logout menu

### 📊 Analytics
- Dashboard with user-specific charts and stats  
- Visual insights on click behavior

### 🔗 UrlShortener
- Form for shortening URLs  
- Success feedback and validation

### 📝 UrlList
- Displays all user URLs  
- Includes click count, copy link, and delete options

---

## ⚙️ Setup Instructions

### 📁 Backend

1. Navigate to the backend folder:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file and add the following:
   ```env
   JWT_SECRET=your-super-secret-jwt-key
   MONGODB_URI=mongodb://localhost:27017/url-shortener
   PORT=5000
   ```
4. Start the backend server:
   ```bash
   npm run dev
   ```

---

### 💻 Frontend

1. Navigate to the frontend folder:
   ```bash
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the frontend server:
   ```bash
   npm run dev
   ```

---

## 🔐 Authentication Flow

- All users must register/login  
- JWT token is stored in localStorage  
- All routes are protected with middleware  
- Each user only accesses their own URLs

---

## 📡 API Endpoints

| Method | Endpoint              | Description                  |
|--------|-----------------------|------------------------------|
| POST   | `/api/auth/register` | Register a new user          |
| POST   | `/api/auth/login`    | Authenticate and get token   |
| POST   | `/api/shorten`       | Shorten a new URL            |
| GET    | `/api/urls`          | Get user's shortened URLs    |
| DELETE | `/api/urls/:id`      | Delete a specific short URL  |

---


