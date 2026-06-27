# Complete Authentication System

A full-stack authentication system built with :contentReference[oaicite:1]{index=1}, :contentReference[oaicite:2]{index=2}, :contentReference[oaicite:3]{index=3}, and :contentReference[oaicite:4]{index=4}.  
This project provides a secure and scalable user authentication flow with email verification, OTP validation, password reset, and JWT-based session management.

---

## Features

- User Registration
- User Login
- Email Verification with OTP
- Forgot Password Functionality
- Reset Password via OTP
- Secure Password Hashing
- JWT Authentication
- Refresh Token Management
- Protected Routes
- Session Handling
- Logout Functionality

---

## Tech Stack

### Frontend
- React.js
- Tailwind CSS
- Axios
- React Router DOM

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT
- bcrypt
- Nodemailer

---

## Project Structure

```bash
complete-authentication-system/
│── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
│── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── services/
│   ├── middlewares/
│   ├── utils/
│   └── server.js
│
└── README.md
```

---

## Installation

### Clone the repository

```bash
git clone https://github.com/Himanshupal15/complete-authentication-system.git
cd complete-authentication-system
```

---

## Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file:

```env
PORT=3000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
EMAIL_USER=your_email
EMAIL_PASS=your_email_password
```

Run backend:

```bash
npm run dev
```

---

## Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

---

## Running Both Frontend & Backend Together

Install concurrently:

```bash
npm install concurrently
```

Add this script in root `package.json`:

```json
"scripts": {
  "dev": "concurrently \"npm run dev --prefix frontend\" \"npm run dev --prefix backend\""
}
```

Run:

```bash
npm run dev
```

---

## API Endpoints

### Auth Routes

| Method | Endpoint | Description |
|---|---|---|
| POST | /api/auth/register | Register user |
| POST | /api/auth/login | Login user |
| POST | /api/auth/verify-otp | Verify OTP |
| POST | /api/auth/forgot-password | Forgot password |
| POST | /api/auth/reset-password | Reset password |
| POST | /api/auth/logout | Logout |

---

## Security Features

- Password hashing using bcrypt
- JWT access & refresh tokens
- OTP expiration handling
- Secure cookies
- Email verification
- Protected routes middleware

---

## Future Improvements

- Google OAuth
- Role-based Authentication
- Two-factor Authentication
- Account Locking after multiple failed attempts
- Profile Management

---

## Author

**Himanshu Pal**

GitHub: https://github.com/Himanshupal15  
LinkedIn: https://www.linkedin.com/in/himanshupal1510/

---

## License

This project is open-source and available under the MIT License.
