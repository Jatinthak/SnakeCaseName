# Project: SnakeCaseName
## Description

Snake Case Name is a simple snake game for beginners. It uses HTML, CSS, and JavaScript to create an engaging user experience.

## Tech Stack

- Frontend: HTML/CSS/JavaScript
- Backend: None (no specific backend required)
- Database: Supabase
- Auth: Supabase
- Payments: Not applicable in this project
- Realtime: False

## Architecture Overview

The architecture of Snake Case Name is a simple game with the following components:

1. **HTML/CSS**: The user interface for playing the game.
2. **JavaScript (ES6+)**: Handles logic and rendering, including snake movement and food spawning.

## API Endpoints

- GET `/api/endpoint`: Returns all endpoints of Snake Case Name
  - Request Body: None
  - Response: JSON with a list of available endpoints

## ENV Variables

- DB_URL: URL to connect to the database (e.g., `postgresql://user:password@localhost/dbname`)
- JWT_SECRET: Secret key for generating secure tokens in Supabase

## Local Setup Instructions

1. Clone this repository from GitHub.
2. Install Node.js and npm if not already installed on your system.
3. Create a new directory to work with the project:
mkdir snake-case-name
cd snake-case-name

4. Initialize a new Node.js project using `npm init`:

   npx create-react-app react-snakelobby --template typescript
   cd react-snakelobby
   npm install @supabase/supabase-js

5. Configure Supabase in the `.env.example` file:
DB_URL=postgresql://user:password@localhost/dbname
JWT_SECRET=mysecretkey
6. Start your local development server with `npm start`.
7. Open a web browser and navigate to http://localhost:3000.

## Deploy Instructions

- For deployment, you can use Docker or AWS Elastic Beanstalk.
  - **Docker**: Build the container using `docker-compose.yml` in this project directory:
    docker-compose up

  - **AWS Elastic Beanstalk**: Create a new application and deploy your code to an Amazon EC2 instance.

## File Structure

- src: Contains all source files for the game.
- public: Static assets like images, stylesheets, etc. are stored here.
- .env.example: Environment variables used in development.
- README.md: Project documentation and setup instructions.
- docker-compose.yml (optional): Local development setup if using Docker.

## Known Issues

1. **Error: "Invalid YAML: while scanning a simple key
  in "<unicode string>", line 33, colu" → Fix: Fixed on attempt 4: Invalid YAML: while scanning a simple key
  in "<unicode string>", line 33, column 20**:
   - This error occurs when trying to parse the JSON response from an API call. It's fixed by adding `response_body` parameter with empty value.
- **Error: "Invalid YAML: while scanning a simple key
  in "<unicode string>", line 18, colu" → Fix: Fixed on attempt 1: Invalid YAML: while scanning a simple key
  in "<unicode string>", line 18, column 20**:
   - This error occurs when trying to parse the JSON response from an API call. It's fixed by adding `response_body` parameter with empty value.

## Conclusion

Snake Case Name is a fun and engaging game for beginners that can be played on your local machine or deployed using Docker or AWS Elastic Beanstalk.
Please note, this project does not include any backend services like database operations or real-time updates.