# Fullstack 2FA (Two-Factor Authentication) Project

This project demonstrates a fully functional **Two-Factor Authentication (2FA)** system using a full-stack approach.  
It enhances user security by requiring both password login and a time-based one-time passcode (TOTP).

## 🔐 Features
- Secure 2FA using TOTP (Time-Based OTP)
- Login authentication using Passport.js
- React-based frontend with clean UI
- Session management using React Context API
- QR code generation for authenticator apps
- Real-time OTP validation
- Full backend + frontend integration

## 📁 Project Structure
backend/  
│── config/  
│── controllers/  
│── models/  
│── routes/  
│── index.js  
client/  
│── src/components  
│── src/pages  
│── src/context  
│── src/service  
│── App.jsx  
│── main.jsx  

## 🖥 Backend Overview
### Tech Stack:
- Node.js
- Express
- Speakeasy (TOTP generation)
- Passport.js (Authentication)
- MongoDB or any DB you configure

### Backend Responsibilities:
- User registration & login
- Generating secret keys
- Creating TOTP codes
- Validating user-entered OTP
- Managing sessions & authentication flows

## 🎨 Frontend Overview
### Tech Stack:
- React
- React Context API (session handling)
- Vite
- Tailwind CSS

### Frontend Responsibilities:
- Login UI
- 2FA code entry page
- QR code display component
- Managing session state
- Calling backend APIs for authentication

## 🔄 How 2FA Works (Flow)
1. User signs up → backend generates a **TOTP secret**
2. Secret is shown as QR code → user scans with Google Authenticator
3. User enters normal password + 6-digit OTP
4. Backend validates OTP using Speakeasy
5. User session is created using React Context

## 🛠 Installation

### Backend:
