# Home Rentals Admin Dashboard

A simple, polished admin dashboard for reviewing Costa Rica rental properties and checking current weather for a selected property location. This project was built as a take-home technical interview submission with a focus on React fundamentals, routing, practical API integration, responsive UI, and clear trade-offs.

## Live Links

- Live demo URL: home-rental-admin-dashboard-g9c1.vercel.app
- GitHub repository: (https://github.com/Kevinrd11/HomeRentalAdminDashboard)

## Tech Stack

- Next.js App Router
- React
- TypeScript
- Plain CSS with responsive, component-oriented classes
- OpenWeatherMap current weather API 
- Browser `localStorage` for demo authentication and Google Identity Services sign-in state

## Features Completed

- Login page with hardcoded demo credentials and optional Sign in with Google through Google Identity Services.
- Friendly validation for missing fields, invalid email format, and invalid credentials.
- Protected dashboard and property detail routes.
- Logout flow that clears the auth flag and redirects to login.
- Responsive property dashboard with five Costa Rica-focused mock rental properties.
- Property detail page with image, address, description, pricing, capacity, and status metadata.
- Reusable weather service that fetches by latitude and longitude.
- Weather loading and error states.
- Deployment-ready environment variable example.

## Demo Login Credentials

```text
Email: admin@homerentals.com
Password: Admin123!
```

## Architecture Decisions

- **Next.js App Router:** Chosen for professional project structure, file-based routing, and straightforward Vercel deployment.
- **TypeScript:** Used to make data models, component props, and weather API responses easier to reason about during review.
- **Frontend-only auth:** The assignment does not require a backend, so authentication is deliberately scoped to a local demo flag in `localStorage`.
- **Client-side weather integration:** Weather is fetched from a reusable service using property coordinates. 
- **Plain CSS:** Avoids extra UI dependencies while still providing a polished responsive admin experience.

## Features Descoped or Simplified Due to the 5-Hour Time Limit

- Backend authentication, server-side Google ID token verification, and secure session management.
- Database persistence for users and properties.
- Admin create, update, and delete workflows.
- Server-side API proxy for weather requests.
- Automated unit/integration tests.
- Role-based permissions.
- Image uploads and asset management.

