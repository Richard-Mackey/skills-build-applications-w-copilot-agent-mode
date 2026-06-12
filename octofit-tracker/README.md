# OctoFit Tracker

A modern multi-tier fitness tracking application built with React 19, Node.js/Express, and MongoDB.

## Architecture

- **Frontend**: React 19 with Vite (Port: 5173)
- **Backend**: Node.js + Express + TypeScript with Mongoose (Port: 8000)
- **Database**: MongoDB (Port: 27017)

## Project Structure

```
octofit-tracker/
├── frontend/          # React 19 + Vite application
│   ├── src/
│   ├── package.json
│   ├── vite.config.ts
│   └── tsconfig.json
└── backend/          # Node.js + Express + TypeScript API
    ├── src/
    ├── package.json
    ├── tsconfig.json
    └── .env.example
```

## Getting Started

### Frontend Setup

```bash
cd octofit-tracker/frontend
npm install
npm run dev
```

The frontend will be available at `http://localhost:5173`

### Backend Setup

```bash
cd octofit-tracker/backend
npm install
cp .env.example .env
npm run dev
```

The backend will be available at `http://localhost:8000`

### Database Setup

Ensure MongoDB is running on `localhost:27017`

```bash
# Example using Docker
docker run -d -p 27017:27017 mongo:latest
```

## Available Scripts

### Frontend
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

### Backend
- `npm run dev` - Start development server with hot reload
- `npm run build` - Compile TypeScript to JavaScript
- `npm start` - Run compiled JavaScript

## Technology Stack

- **Frontend**: React 19, TypeScript, Vite
- **Backend**: Node.js, Express, TypeScript, Mongoose
- **Database**: MongoDB
- **Tools**: ESLint, Cors

## Environment Variables

Create a `.env` file in the backend directory with the following variables:

```
BACKEND_PORT=8000
MONGODB_URI=mongodb://localhost:27017/octofit-tracker
```