# 🔐 NextAuth Authentication System

A full-stack authentication system built with **Next.js**, **NextAuth.js**, **MongoDB**, and **bcrypt**.

The project implements secure user registration and login using both traditional email/password authentication and Google OAuth. It also demonstrates JWT-based sessions, protected routes, middleware authentication, and deployment on Vercel.

---

## 🚀 Features

- 🔑 User registration with email and password
- 🔐 Secure password hashing using bcrypt
- 📧 Credentials-based authentication
- 🌐 Google OAuth authentication
- 🍪 JWT-based session management
- 🛡️ Protected routes using Next.js Middleware
- 🔄 Callback URL support after authentication
- 👤 User information stored in MongoDB
- ☁️ Vercel deployment support
- 🔒 Environment variable based configuration
- 📡 API routes using Next.js App Router

---

## 🛠️ Tech Stack

### Frontend
- Next.js
- React
- TypeScript
- Tailwind CSS

### Backend
- Next.js App Router
- Next.js API Routes
- NextAuth.js
- MongoDB
- Mongoose

### Authentication & Security
- NextAuth.js
- JWT
- bcrypt
- Google OAuth
- HTTP-only authentication cookies
- Middleware-based route protection

### Deployment
- Vercel
- GitHub

---

## 📂 Project Structure

```text
src/
│
├── app/
│   ├── api/
│   │   ├── auth/
│   │   │   ├── [...nextauth]/
│   │   │   │   └── route.ts
│   │   │   └── register/
│   │   │       └── route.ts
│   │   │
│   │   ├── edit/
│   │   │   └── route.ts
│   │   │
│   │   └── user/
│   │       └── route.ts
│   │
│   ├── edit/
│   │   └── page.tsx
│   │
│   ├── login/
│   │   └── page.tsx
│   │
│   ├── register/
│   │   └── page.tsx
│   │
│   └── page.tsx
│
├── context/
│   └── UserContext.tsx
│
├── lib/
│   ├── auth.ts
│   ├── cloudinary.ts
│   └── db.ts
│
├── models/
│   └── User.ts
│
└── middleware.ts
