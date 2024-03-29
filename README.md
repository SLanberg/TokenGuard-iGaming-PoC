# TokenGuard

## Initial installation

# Docker (System with no Docker Desktop)
1) Go to the root folder of the project
2) docker compose up

# Installation with .env files
1) Create 2 .env files in front-end and back-end folder
  
2) In Back-End .env file write in:
`PGUSER=postgres
PGHOST=127.0.0.1
PGPASSWORD="123"
PGDATABASE=tokenguard
PGPORT=5432`

3) In the Back-End folder run `npx tsx src/index.ts`

In Front-End .env file write in:
1) VITE_APP_MY_BACKEND: `http://localhost:8000/api`
   
2) In the Front-End folder run `npm run dev`

3) In the DB create tables with the commands from the init.sql or import it

## Run tests
1) Go the the /front-end folder
2) Run `npm test`

## Format with prettier
1) npx prettier --write .

## Technology description
For the front-end used: SvelteKit, Tailwind, TypeScript
For the back-end used: Node.js, Postgres, TypeScript
Wrapped in the Docker.
