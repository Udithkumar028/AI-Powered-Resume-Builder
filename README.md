# AI Powered Resume Builder

This repository contains a full-stack AI-powered resume builder (React + Node/Express + MongoDB) with local development scripts.

## Features

- Resume creation and editing UI (React + Vite)
- PDF generation using `@react-pdf/renderer`
- AI-powered suggestions and ATS scoring (server-side services)
- Authentication and versioning of resumes

## Repo layout

- `client/` - React frontend (Vite)
- `server/` - Express backend (Node.js)

## Prerequisites

- Node.js (>=16) and `npm`
- A MongoDB database (Atlas or self-hosted)
- Google OAuth credentials (if using Google sign-in)
- Optional: Gemini / AI provider API key for AI features

## Environment

Create a `.env` file in the `server/` directory with the following keys (example):

```
MONGO_URI=your_mongodb_connection_string
PORT=5000
JWT_SECRET=your_jwt_secret
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
GEMINI_API_KEY=your_gemini_or_ai_key
NODE_ENV=development
```

## Local setup

1. Clone the repo

```bash
git clone https://github.com/Udithkumar028/AI-Powered-Resume-Builder.git
cd "AI Powered Resume Builder"
```

2. Install server dependencies

```bash
cd server
npm install
```

3. Install client dependencies

```bash
cd ../client
npm install
```

4. Create `server/.env` (see Environment section)

5. Start the backend and frontend (in separate terminals)

```bash
# Terminal 1 — server
cd server
npm run dev

# Terminal 2 — client
cd client
npm run dev
```

The client will be available at `http://localhost:5173/` (or another port if 5173 is occupied). The server runs on the port set in `PORT` (default 5000).

## Production build

Build the client and serve static files from a host of your choice:

```bash
cd client
npm run build

# Serve `client/dist` from your static host or integrate with the Express server
```

## Pushing changes to GitHub

I have already pushed this repository to `https://github.com/Udithkumar028/AI-Powered-Resume-Builder`. To push further changes:

```bash
git add .
git commit -m "Your message"
git push
```

## Contact

If you need help, contact: udithkumar028@gmail.com

---

Thanks for using the AI Powered Resume Builder — let me know if you want GitHub Actions, a PR template, or a license file added.
