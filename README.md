# Unfazed — MERN Major Project

A starter implementation of the Unfazed therapist-practice platform described in the supplied project brief.

## Stack
- Frontend: React + Vite + React Router + Axios
- Backend: Node.js + Express + Mongoose
- Authentication: bcryptjs + JWT
- Optional integrations prepared for Razorpay and Socket.io

## Requirements
Node.js 18+, npm, and a MongoDB database (local or Atlas).

## Setup

### 1. Backend
```bash
cd unfazed-backend
cp .env.example .env
npm install
npm run dev
```

Set `MONGO_URI` and a strong `JWT_SECRET` in `.env`.

### 2. Frontend
In another terminal:
```bash
cd unfazed-frontend
cp .env.example .env
npm install
npm run dev
```

Open the Vite URL shown in the terminal (normally http://localhost:5173).

## Included in this starter
- Therapist registration and login
- JWT-protected therapist profile endpoint
- Public therapist profile route by slug
- Basic React login/register/dashboard screens
- MongoDB models and API structure for the remaining project modules
- Centralized entitlement-service scaffold
- Scheduling, CRM, payments, notes, chat and analytics route/service placeholders

## Important
This is a runnable foundation, not a production-ready clinical system. The remaining modules need implementation and testing before submission. Do not store real patient/clinical data in this starter. Add validation, authorization tests, audit logging, privacy controls, secure deployment configuration, and payment webhook verification before production use.

## Suggested development order
1. Complete availability and double-booking prevention.
2. Add client CRM, intake and consent.
3. Add Razorpay order creation and signature/webhook verification.
4. Enforce private/shared note separation at the API layer.
5. Add Socket.io chat and notification events.
6. Complete tier configuration, entitlement gates and MongoDB aggregation analytics.
