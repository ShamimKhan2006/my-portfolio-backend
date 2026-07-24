# Backend Setup

The backend is built with Node.js and Express.js, and serves as the API layer for the portfolio's contact form.

## Folder Structure

```
backend/
  server.js        # Express server
  .env             # Environment variables
  package.json     # Backend dependencies
```

## Setup

```bash
cd backend
npm install
```

## Environment Variables

Create a `.env` file inside the `backend` folder:

```env
PORT=5000
EMAIL_SERVICE=gmail
EMAIL_USER=mdshamim200616@gmail.com
EMAIL_PASS=your_app_password_here
CONTACT_EMAIL=mdshamim200616@gmail.com
```

For Gmail, use an app password instead of your main password.

## Run the Backend

```bash
# From project root
npm run server

# Or from backend folder
cd backend
node server.js
```

The backend API will be available at `http://localhost:5000/api/contact`.

## Run Full Stack

```bash
npm run dev:all
```

This starts:
- Next.js frontend on `http://localhost:3000`
- Express backend on `http://localhost:5000`

## API Endpoints

| Method | Endpoint       | Description               |
|--------|----------------|---------------------------|
| POST   | `/api/contact` | Submit contact form       |
| GET    | `/api/health`  | Health check              |
