# PassTheSalt

PassTheSalt is a full stack web application I built as a side project for colleagues at SALT (School of Applied Technology).

The idea behind the project was to create a shared platform where students and colleagues could manage courses, collaborate in teams, share feedback and organize social activities.

The application combines a Java and Spring Boot backend with a React and TypeScript frontend.

## Features

- Course creation and management
- Course schedules and user assignments
- Mob programming group management
- Retrospectives and feedback
- Anonymous questions
- Afterwork events and location voting
- Separate dashboards for admins, users and mob groups
- REST APIs for communication between frontend and backend
- PostgreSQL database for storing application data

## Tech Stack

### Backend
- Java 17
- Spring Boot
- Spring Data JPA
- Spring Security
- REST APIs
- Maven

### Frontend
- React
- TypeScript
- Vite
- Tailwind CSS
- TanStack Router
- TanStack Query

### Database
- PostgreSQL

### Deployment
- Railway for backend hosting
- GitHub Pages for frontend hosting
- GitHub Actions for deployment workflows

## Project Structure

```text
PassTheSalt/
├── backend/
│   ├── src/
│   └── pom.xml
├── frontend/
│   ├── src/
│   ├── package.json
│   └── vite.config.ts
├── SETUP.md
├── DEPLOYMENT.md
└── README.md
```

## Getting Started

### Requirements

Make sure you have the following installed:

- Java 17
- Maven 3.8+
- Node.js 18+
- PostgreSQL

### 1. Clone the repository

```bash
git clone https://github.com/venulehtonen/PassTheSalt.git
cd PassTheSalt
```

### 2. Set up the database

Create a PostgreSQL database named `passthesalt`.

Configure the following environment variables for the backend:

```env
PGHOST=localhost
PGPORT=5432
PGDATABASE=passthesalt
PGUSER=postgres
PGPASSWORD=your_password
```

Set these in your terminal or development environment before starting the backend.

### 3. Start the backend

```bash
cd backend
mvn spring-boot:run
```

The backend runs at:

`http://localhost:8080`

### 4. Start the frontend

Open another terminal.

```bash
cd frontend
npm install
npm run dev
```

The frontend runs at:

`http://localhost:3001`

## Deployment

The project includes deployment documentation for Railway and GitHub Pages.

For more details, see [DEPLOYMENT.md](DEPLOYMENT.md) and [SETUP.md](SETUP.md).

## About the Project

I created PassTheSalt to put my full stack development skills into practice while building something useful for people around me.

Working on the project gave me practical experience connecting a React frontend with a Spring Boot backend, designing REST APIs, working with PostgreSQL and developing features based on real user needs.

It was also an opportunity to combine two things I enjoy: technology and bringing people together.

## Author

**Venujan Nagendirakumar**

Full Stack Developer

[GitHub](https://github.com/venulehtonen)
