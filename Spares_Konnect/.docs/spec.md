# Spares Konnect - Project Specification & Architecture

## 1. Objective
Transform the repository structure from a standalone React + Vite template into a full-stack monorepo supporting the backend API and frontend client outlined in the project README[cite: 2].

## 2. Directory Structure Changes
Create the following directory layout without altering unrelated files:
```text
spares-konnect/
├── client/                 # Existing React + Vite frontend files moved/kept here
├── server/                 # New Node.js / Express backend
│   ├── config/             # DB connection pool
│   ├── controllers/        # Business logic
│   ├── middleware/         # JWT auth middleware
│   └── routes/             # API route definitions
├── .env.example            # Environment variables template
└── package.json            # Root workspace or runner scripts