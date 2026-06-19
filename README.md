# Prescripto Full Stack

A full-stack medical appointment booking application with separate admin, backend, and frontend modules.

## Project Structure

- `admin/` — admin panel source and configuration
- `backend/` — Node.js/Express API server and MongoDB configuration
- `frontend/` — public-facing React application
- `How_To_Run_Project.pdf` — optional PDF guide for running the project

## Key Features

- Admin dashboard for managing doctors, appointments, and users
- Doctor and user authentication
- Appointment booking and profile management
- Responsive frontend built with React and Tailwind CSS

## Prerequisites

- Node.js 18+ recommended
- npm
- MongoDB database
- Git (for repository management)

## Setup and Run

### 1. Install dependencies

Open a terminal inside each folder and run:

```bash
cd admin
npm install

cd ../backend
npm install

cd ../frontend
npm install
```

### 2. Configure environment variables

Create `.env` files in the following folders as needed:

- `admin/`
- `backend/`
- `frontend/`

Typical environment settings include API endpoints, database URI, JWT secrets, and cloudinary credentials.

> Note: `.env` files are excluded from Git by `.gitignore`.

### 3. Start the backend

```bash
cd backend
npm run server
```

### 4. Start the frontend apps

Open two separate terminals:

```bash
cd frontend
npm run dev
```

```bash
cd admin
npm run dev
```

## Folder Details

### `admin/`

- `src/` — admin panel React source code
- `public/` — static assets for admin interface
- `vite.config.js`, `tailwind.config.js` — tooling config

### `backend/`

- `server.js` — Express app entry point
- `routes/` — API route definitions
- `controllers/` — request handlers
- `models/` — Mongoose schemas
- `middleware/` — authentication and file upload middleware
- `config/` — MongoDB and Cloudinary setup

### `frontend/`

- `src/` — main React app source
- `components/` — shared UI components
- `pages/` — public website pages
- `assets/` — images and icons

## GitHub Updates

This repository is already initialized and linked to GitHub. Use the commands below to keep it synced:

```bash
git add .
git commit -m "Your message"
git push origin main
```

## Notes

- Keep secrets out of source control
- Use `.gitignore` to avoid committing sensitive files and generated artifacts
- If you change the backend port or API base path, update the frontend and admin environment configs accordingly

---

Built with React, Tailwind CSS, Vite, Express, and MongoDB.
