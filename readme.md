![License](https://img.shields.io/badge/License-MIT-blue)
![Node](https://img.shields.io/badge/Node.js-18%2B-green)
![MongoDB](https://img.shields.io/badge/Database-MongoDB%20Atlas-success)
![React](https://img.shields.io/badge/Frontend-React.js-blue)
![JWT](https://img.shields.io/badge/Auth-JWT-orange)
![Express](https://img.shields.io/badge/Backend-Express.js-lightgrey)
![Tailwind](https://img.shields.io/badge/UI-TailwindCSS-38BDF8)


# 🔐 Advanced MERN Authentication System

A full-featured **Authentication System** built with the **MERN stack** — complete with **user registration, email verification, OTP-based security, JWT authentication, password recovery, and role-based access**.  
This project follows modern authentication standards with `bcrypt` password hashing, `JWT` tokens, and `NodeMailer` email verification.

---

## 🚀 Features

✅ **User Registration & Login**  
✅ **Email Verification via OTP**  
✅ **Forgot Password / Reset Password**  
✅ **Change Password (Authenticated users)**  
✅ **Secure Password Hashing (bcrypt)**  
✅ **JWT-based Authentication & Authorization**  
✅ **Error Handling & Token Expiry Validation**  
✅ **Protected Routes (Frontend + Backend)**  
✅ **Responsive UI with Glassmorphism Theme**  
✅ **Environment Variable Configuration for Security**  

---

## 🧩 Tech Stack

| Layer | Technologies |
|--------|---------------|
| **Frontend** | React.js, Vite, Tailwind CSS |
| **Backend** | Node.js, Express.js |
| **Database** | MongoDB (Mongoose ORM) |
| **Authentication** | JWT (JSON Web Token), bcrypt |
| **Email Service** | NodeMailer (SMTP / Gmail) |
| **Validation** | Express Validator / Custom OTP Logic |

---

## 🗂️ Folder Structure

<details>
<summary>📁 Click to expand project structure</summary>

```bash
MERN-AUTH/
│
├── backend/
│   ├── config/              # DB and Passport configuration
│   ├── controllers/         # Auth logic (register, login, OTP, etc.)
│   ├── middleware/          # Auth & error middlewares
│   ├── models/              # Mongoose user schema
│   ├── routes/              # Express routes
│   ├── utils/               # Email sending, token helpers
│   └── server.js            # App entry point
│
└── frontend/
    ├── src/
    │   ├── components/      # UI Components (Forms, Navbar, Buttons, etc.)
    │   ├── pages/           # Auth pages (Register, Login, OTP, Forgot Password)
    │   ├── context/         # Auth Context + Protected Routes
    │   ├── App.jsx
    │   └── index.css        # Cyber Warm Glassmorphism Theme ✨
    │
    ├── package.json
    └── vite.config.js
```
</details>


## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/ShreyaPandayy/MERN-AUTH.git
cd mern-auth
```
2️⃣ Backend Setup
```bash
cd backend
npm install
```

Create a .env file inside /backend and add:
```bash
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key

EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_app_password
CLIENT_URL=http://localhost:5173
```

Start backend:
```bash
npm start
```

3️⃣ Frontend Setup
```bash
cd ../frontend
npm install
npm run dev
```

Visit: http://localhost:5173

🔑 Authentication Flow

1️⃣ Register: User signs up → OTP sent to email
2️⃣ Verify Email: User enters OTP → account verified
3️⃣ Login: Authenticated via JWT token
4️⃣ Forgot Password: OTP sent to reset email
5️⃣ Change Password: Authenticated users can change their password

🔒 Security Highlights
```bash
Passwords are hashed using bcrypt

JWT tokens include user ID & expiry time

Email verification prevents fake accounts

OTP expires after a fixed duration

Protected API routes verify token validity
```

🎨 UI Theme
```bash

This project uses a Cyber Warm Glassmorphism design built with Tailwind CSS:

Futuristic warm amber + magenta tones

Blurred translucent cards

Smooth gradients and hover glow effects
```
🧰 Future Enhancements
```

Add Google / GitHub OAuth Login

Enable Refresh Tokens

Implement Role-based Admin Access

Deploy to Render / Vercel (Full-stack Deployment)
```


🪄 License
```
This project is open-source under the MIT License.
Feel free to fork and enhance it!
```
```
“Secure code, seamless experience — authentication done right.” 🔐
— Shreya Pandey
```



