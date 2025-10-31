# Cloud-kitchen````markdown
# Cloud Kitchen (Node.js + MySQL)

A minimal Cloud Kitchen web app using Node.js, Express, EJS and MySQL.

Features
- User registration and login
- View menu
- Place orders
- View your orders
- Simple admin dashboard placeholder

Prerequisites
- Node.js 18+ and npm
- MySQL server

Quick start
1. Clone repo (or create a new project) and add these files.
2. Install dependencies:
   npm install
3. Create a database and import schema:
   - Create a MySQL database (example name: cloud_kitchen)
   - Run the SQL in `db/schema.sql` (mysql -u user -p cloud_kitchen < db/schema.sql)
4. Create a `.env` from `.env.example` and set your DB credentials and session secret.
5. Start the app:
   npm run dev
6. Open: http://localhost:3000

Notes
- Passwords are hashed with bcrypt.
- Uses mysql2/promise and prepared statements.
- This is a minimal scaffold. Add validation, CSRF, input sanitization, helmet, HTTPS, and production session store before deploying.
