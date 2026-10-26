# Deposit Return Investment Desk

## One-sentence benefit
Helps packaging teams, municipalities and investors coordinate deposit-return infrastructure, collection targets and recycling finance.

## Live demo
Run the Java service and Vue application locally to use the complete experience.

## Screenshots
![deposit return investment workspace](docs/screenshot.png)

## Main features
Search return schemes, add a realistic pilot, progress evidence, inspect priorities and open dedicated system guidance.

## Technology used
Vue, TypeScript, Pinia, Vue Router, Vite, Spring Boot and Java.

## Installation instructions
Start the backend with `cd backend && mvn spring-boot:run`. In another terminal run `npm install && npm run dev`.

## Commercial licensing/contact
Commercial licensing and implementation support are available through the repository owner.

## Business problem and users
Producers, retailers, system operators and investors need a clear way to coordinate return-point coverage, collection evidence and accountable owners.

## Key workflows
Users can filter return schemes, create a Brussels pilot, move a scheme forward and review system guidance.

## Vue framework highlights
The application uses the Composition API, Pinia computed state, reactive filters and Vue Router pages.

## Java backend highlights
The Spring Boot service provides real list, search, create and update endpoints, validation, clear errors, health reporting and tests.

## Architecture and state flow
Pinia owns the shared client state and synchronises it with the Java API after reads and writes.

## Accessibility and responsive behaviour
Landmarks, labels, visible focus, readable status text and responsive panels support keyboard and mobile users.

## Verification commands
Use `npm test`, `npm run build`, and `cd backend && mvn test package`.

## Structure
`src` contains the Vue experience, `backend` contains the Java service, and `docs` contains verified media.

## Tradeoffs
The demonstration uses an in-memory data store; production deployment would add authentication, persistence and producer-responsibility finance integrations.

## Roadmap
Add container-flow baselines, deposit-value checks, consumer access safeguards, recycler verification and durable storage.
