# Project Brain SnakeCaseName
## Description

Snake Case Name is a simple snake game built using HTML, CSS, JavaScript (React), Node.js, Python Flask, and PostgreSQL. The frontend uses React for the user interface while the backend runs on Node.js with Flask to handle HTTP requests.

## Tech Stack

- **Frontend**: React + NextJS
- **Backend**: Node.js + FastAPI or Django
- **Database**: PostgreSQL
- **Auth**: Supabase
- **Payments**: None
- **Realtime**: True

## Architecture Overview (Text Diagram)

![Snake Case Name Architecture](https://github.com/yourusername/SnakeCaseName/blob/main/docs/architecture.png?raw=true "Snake Case Name Architecture")

## API Endpoints from Contract

The following endpoints are defined in the contract:

1. GET /api/users
2. POST /api/login
3. PUT /api/user/{id}
4. DELETE /api/user/{id}

## Environment Variables (ENV)

- **DB_URL**: The URL for your PostgreSQL database.
- **JWT_SECRET**: A secret key used to sign JWT tokens.

## Local Setup Instructions

1. Clone the repository: `git clone https://github.com/yourusername/SnakeCaseName.git`
2. Install dependencies using npm or yarn (`npm install` or `yarn add`)
3. Start development server with Docker Compose (if local setup): `docker-compose up -d`

## Deploy Instructions

1. Set up a production environment for your backend and database.
2. Configure Supabase to handle user authentication.

### File Structure
- **docs** contains project documentation, including README.md.
- **src** is the main source code repository with React components, NextJS app, Node.js server, Flask apps, etc.
- **public/**: static files like images and stylesheets for frontend.
- **.env.example**: environment variables template.

## License

This project follows [MIT](https://github.com/yourusername/SnakeCaseName/blob/main/LICENSE) license terms.