# Legacy OFS — Field Ticketing and Inspections

Legacy OFS is a mobile-friendly field ticketing application for oilfield service operations.

## Features

- Field ticket creation and management
- Configurable ticket templates
- PostgreSQL-based ticket storage
- Ticket status workflow
- Administrative review and approval
- Planned offline support and synchronization

## Technology Stack

- Frontend: React
- Backend: Node.js and Express
- Database: PostgreSQL
- Version Control: Git and GitHub

## Project Structure

- `frontend/` — React application
- `backend/` — Express API and database connection
- `README.md` — Project documentation
- `CODE_REVIEW.md` — Code review notes
- `TEST_PLAN.md` — Test cases and verification results

## Setup

### Backend

1. Open the backend directory.
2. Install dependencies with `npm install`.
3. Configure the database connection and environment variables.
4. Start the server using the configured npm script or `node server.js`.

### Frontend

1. Open the frontend directory.
2. Install dependencies with `npm install`.
3. Start the development server with `npm run dev`.

Use the actual database name, local ports, and environment variable names from your project configuration.

## API Endpoints

- `GET /` — Backend status
- `GET /api/health` — Database health check
- `GET /api/tickets` — List tickets
- `POST /api/tickets` — Create a ticket
- `PATCH /api/tickets/:id/status` — Update ticket status

## Technical Decisions

React, Express, and PostgreSQL are used to separate the user interface, application logic, and persistent storage. Parameterized SQL queries and server-side input validation improve security and reliability.

## Security and Limitations

Never commit real secrets or database passwords. Administrative routes must enforce server-side authentication and authorization. Offline synchronization, audit logging, and automated test coverage require additional validation.


