# MERN Stack Boilerplate

A full-stack MERN (MongoDB, Express, React, Node.js) application boilerplate with separate backend and frontend directories.

## Project Structure

```
mern-app/
├── backend/          # Express.js server
│   ├── config/       # Database configuration
│   ├── middleware/   # Custom middleware
│   ├── models/       # Mongoose models
│   ├── routes/       # API routes
│   ├── utils/        # Utility functions
│   ├── server.js     # Entry point
│   ├── .env          # Environment variables
│   └── package.json
├── frontend/         # React + Vite client
│   ├── src/          # React source code
│   ├── .env          # Environment variables
│   ├── vite.config.js
│   ├── tailwind.config.js
│   └── package.json
├── node_modules/     # Root dependencies
├── package.json      # Root scripts
└── package-lock.json
```

## Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- MongoDB (local or MongoDB Atlas)
- Git

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/rop2024/asset-template-mern-stack.git
cd asset-template-mern-stack
```

### 2. Install dependencies

Install root dependencies:

```bash
npm install
```

Install backend dependencies:

```bash
npm run install-server
```

Install frontend dependencies:

```bash
npm run install-client
```

Or install everything at once:

```bash
npm run install-all
```

### 3. Configure environment variables

#### Backend

Create a `.env` file in the `backend/` directory:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
NODE_ENV=development
```

#### Frontend

Create a `.env` file in the `frontend/` directory:

```
VITE_API_URL=http://localhost:5000
```

### 4. Run the application

#### Development mode (runs both server and client concurrently)

```bash
npm run dev
```

#### Run only the backend server

```bash
npm run server
```

#### Run only the frontend client

```bash
npm run client
```

The backend server will run on `http://localhost:5000` and the frontend client on `http://localhost:5173` (default Vite port).

## Available Scripts

| Script | Description |
|--------|-------------|
| `npm run dev` | Run backend and frontend concurrently in development |
| `npm run server` | Start the backend server |
| `npm run client` | Start the frontend client |
| `npm run install-server` | Install backend dependencies |
| `npm run install-client` | Install frontend dependencies |
| `npm run install-all` | Install all dependencies (server + client) |

## Backend Scripts

| Script | Description |
|--------|-------------|
| `npm start` | Start production server |
| `npm run dev` | Start server with nodemon (auto-restart) |

## Frontend Scripts

| Script | Description |
|--------|-------------|
| `npm run dev` | Start Vite dev server |
| `npm run build` | Build for production |
| `npm run lint` | Run ESLint |
| `npm run preview` | Preview production build |

## Tech Stack

- **Backend**: Node.js, Express, MongoDB, Mongoose, JWT, bcryptjs, CORS, dotenv, Morgan, Express Validator
- **Frontend**: React 18, Vite, Tailwind CSS, Axios, PostCSS
- **DevTools**: Concurrently, Nodemon, ESLint

## License

ISC