# Getting Started

Follow these steps to run the project locally.

## Prerequisites

- Node.js >= 18
- .NET 9 SDK
- Docker & Docker Compose
- PostgreSQL or SQLite

## Setup Frontend

```bash
cd frontend
npm install
npm run dev
```

Frontend will run on http://localhost:3000.

## Setup Backend

```bash
cd backend
dotnet restore
dotnet run
```

API will run on http://localhost:5000.

## Dockerized Version

Run both frontend and backend together:

```bash
docker-compose up --build
```

The full app will be available at http://localhost:3000.


