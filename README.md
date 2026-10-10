# Spares Konnect 🚗🔧

Spares Konnect is a specialized software platform designed to support local garage owners and independent mechanics. It bridges the operational gap between automotive repair shops and spare parts management by streamlining inventory tracking, supplier coordination, and job-cost oversight in a single dashboard.

## Core Features

- Job-linked inventory: track every part received, reserved, used, returned, or sold against an individual repair job card.
- Real-time stock management: monitor inventory levels and receive alerts for low stock on fast-moving parts.
- Supplier marketplace linkage: connect garages with local spare parts dealers to simplify ordering and price comparison.
- Audit and returns trail: record returns, core charges, and warranty replacements to reduce end-of-month discrepancies.

## Tech Stack

### Frontend
- React.js
- Tailwind CSS
- Mobile-friendly layout for workshop use

### Backend
- Node.js with Express
- Python with FastAPI

### Database
- PostgreSQL
- MongoDB

### Authentication
- JWT
- OAuth2

## Getting Started for Developers

Follow these instructions to set up, build, and run the project locally for development and testing.

### Prerequisites

Ensure the following are installed on your system:

- Node.js (v18 or newer recommended)
- Git
- A package manager such as npm, yarn, or pnpm
- A running database instance, such as PostgreSQL or MongoDB

### 1. Clone the repository

```bash
git clone https://github.com/your-username/spares-konnect.git
cd spares-konnect
```

### 2. Configure the environment

Create a `.env` file in the project root (or in separate client/server directories if using a monorepo) based on the provided template:

```bash
cp .env.example .env
```

Update the environment variables to match your local configuration, including database URIs, ports, and JWT secrets.

### 3. Install dependencies

Install the required dependencies for the application:

```bash
npm install
```

If your project includes a separate frontend client, install those dependencies as well:

```bash
cd client
npm install
cd ..
```

### 4. Run the application

Start the backend server:

```bash
npm run dev
```

In a separate terminal, start the frontend client:

```bash
cd client
npm run start
```

The application should now be running locally at:

- Frontend: http://localhost:3000
- Backend API: http://localhost:5000

## Contributing Guidelines

We welcome contributions from developers, mechanics, and automotive enthusiasts. To contribute:

1. Fork the repository and create a feature branch.

```bash
git checkout -b feature/amazing-feature
```

2. Commit your changes.

```bash
git commit -m "Add some amazing feature"
```

3. Push the branch to your fork.

```bash
git push origin feature/amazing-feature
```

4. Open a pull request describing your changes and how they benefit local garages and mechanics.

