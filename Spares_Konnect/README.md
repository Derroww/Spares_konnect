# Spares Konnect 🚗🔧

Spares Konnect is a specialized software platform designed to support local garage owners and independent mechanics. It connects automotive repair shops with spare parts management by streamlining inventory tracking, supplier coordination, and job-cost oversight in a single dashboard.

## Features

- Job-linked inventory tracking for every part received, reserved, used, returned, or sold against a repair job card
- Real-time stock monitoring with low-stock alerts for fast-moving items
- Supplier marketplace integration to simplify ordering and price comparison
- Audit and returns tracking for warranty replacements, core charges, and end-of-month reconciliation

## Tech Stack

### Frontend
- React.js
- Vite
- Tailwind CSS
- Mobile-friendly workshop dashboard

### Backend
- Node.js
- Express.js
- REST API architecture

### Database
- PostgreSQL

### Authentication
- JWT (JSON Web Tokens)

## Project Architecture

This project is structured as a monorepo with separate frontend and backend directories to keep the client application and API services clearly separated.

```text
spares-konnect/
├── client/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
├── server/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── routes/
│   ├── .env.example
│   ├── package.json
│   └── server.js
├── README.md
├── LICENSE
└── ...
```

## Getting Started

### Prerequisites

Make sure the following are installed on your machine:

- Node.js (v18 or newer recommended)
- Git
- npm, yarn, or pnpm
- PostgreSQL database instance

### 1. Clone the repository

```bash
git clone https://github.com/your-username/spares-konnect.git
cd spares-konnect
```

### 2. Configure environment variables

Create a `.env` file inside the `server/` directory based on the example template:

```bash
cd server
cp .env.example .env
```

Update the values in `server/.env` to match your local setup, including:

- `PORT`
- `DATABASE_URL`
- `JWT_SECRET`

### 3. Install dependencies

#### Backend

```bash
cd server
npm install
```

#### Frontend

```bash
cd ../client
npm install
```

### 4. Run the application locally

Start the backend server in one terminal:

```bash
cd server
npm run dev
```

Start the frontend client in another terminal:

```bash
cd client
npm run dev
```

The app should be available at:

- Frontend: `http://localhost:3000`
- Backend API: `http://localhost:5000`

## Contributing

We welcome contributions from developers, mechanics, and automotive enthusiasts.

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Commit your work
5. Push to your fork
6. Open a pull request

### Example

```bash
git checkout -b feature/amazing-feature
git commit -m "Add some amazing feature"
git push origin feature/amazing-feature
```