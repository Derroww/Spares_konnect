### File 2: `AGENTS.md` (Coding Agent Execution Instructions)
```markdown
# Agent Instructions: Executing Repository Alignment

## Task Overview
Your task is to fix the project setup gap by introducing the backend server structure and aligning the repository scripts with the architecture defined in `README.md`[cite: 2].

## Step-by-Step Execution Plan

### Step 1: Create Backend Directory & Configuration
1. Create a `server/` folder at the root.
2. Initialize `server/config/db.js` using the `pg` pool module connecting via `process.env.DATABASE_URL`.
3. Add `server/middleware/authMiddleware.js` for token verification using `jsonwebtoken`.

### Step 2: Implement API Routes & Controllers
1. Create `server/controllers/authController.js` and `server/routes/authRoutes.js` for user registration and login.
2. Create `server/controllers/jobController.js` and `server/routes/jobRoutes.js` to handle job-linked spare parts tracking (reserved, used, returned, sold).
3. Create `server/server.js` as the main entry point connecting Express middleware, CORS, and route handlers.

### Step 3: Update Package Scripts & Environment
1. Add a root `package.json` (or update existing) to manage scripts for running both client and server concurrently if desired.
2. Create `.env.example` specifying required environment variables:
   ```env
   PORT=5000
   DATABASE_URL=postgresql://user:password@localhost:5432/spares_konnect_db
   JWT_SECRET=your_jwt_secret