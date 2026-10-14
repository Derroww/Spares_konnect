# System Architecture: Spares Konnect

## 1. Tech Stack Alignment
- **Frontend:** React.js with Tailwind CSS, built via Vite for optimal client performance.
- **Backend API:** Node.js & Express.js REST API architecture handling business logic and authorization[cite: 2].
- **Database:** PostgreSQL relational database managing multi-tenant garage data, parts, and job linkages[cite: 2].

## 2. Relational Data Model (Core Entities)
- **Users:** Stores system users (mechanics, managers, admins) with role-based permissions.
- **Parts:** Master inventory table containing SKU, part name, category, unit cost, and current stock level.
- **Job Cards:** Active repair tracking records tied to specific vehicles and clients.
- **Job Parts (Join Table):** Maps parts movement to job cards, capturing `quantity`, `status` (reserved, used, returned, sold), and timestamps.