# FoodLab Frontend

FoodLab Frontend is a React single-page application for a modern restaurant/food service experience. It showcases marketing pages, menu exploration, search, reservation-focused sections, and a lightweight personal login/dashboard flow.

## Overview

This project was built with:

- **React 18**
- **React Router v6** for routing
- **Bootstrap + React-Bootstrap** for UI and layout
- **Axios** for HTTP requests
- **JSON Server** for local mock APIs

## Main Features

- Multi-page style navigation in an SPA:
  - Home
  - About
  - Services
  - Menu
  - Contact
- Search page with dynamic route parameter (`/search/:searchValue`)
- Personal login page (`/personal-page`)
- User dashboard route (`/dashboard/:id`)
- Reusable UI components (Navbar, Footer, cards, buttons, shopping cart UI)

## Project Structure

```text
foodlab/
├── database/
│   ├── products.json
│   └── personalData.json
├── src/
│   ├── assets/
│   ├── components/
│   │   ├── Pages/
│   │   └── Template/
│   ├── data/
│   ├── functions/
│   ├── hooks/
│   ├── App.js
│   └── index.js
├── package.json
└── README.md
```

## Prerequisites

- **Node.js** 18+ (recommended)
- **npm** 9+ (or compatible)

## Getting Started

1. Clone the repository.
2. Move into the project directory:

   ```bash
   cd foodlab
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

## Running the Application (Development)

To run the frontend:

```bash
npm start
```

By default, Create React App runs on:

- `http://localhost:3000`

## Running Mock API Servers

This project includes local JSON mock data and two dedicated scripts.

Start products API:

```bash
npm run products-server
```

- Default endpoint base: `http://localhost:3001`

Start personal data API:

```bash
npm run personal-data-server
```

- Default endpoint base: `http://localhost:3003`

> Recommended: run the frontend and both mock servers in separate terminals for full local functionality.

## Available Scripts

From `foodlab/package.json`:

- `npm start` — Runs the app in development mode.
- `npm run build` — Builds the app for production.
- `npm test` — Launches test runner in interactive watch mode.
- `npm run eject` — Ejects CRA configuration (irreversible).
- `npm run products-server` — Starts JSON Server for product data.
- `npm run personal-data-server` — Starts JSON Server for personal data.

## Routing Summary

Configured routes include:

- `/`
- `/about`
- `/services`
- `/menu`
- `/contacts`
- `/search/:searchValue`
- `/personal-page`
- `/dashboard/:id`

## Build for Production

Create optimized production build:

```bash
npm run build
```

The output is generated in the `build/` directory.

## Tech Notes

- The application uses a component-driven structure with reusable template components.
- Bootstrap styling is globally imported from `App.js`.
- Local mock APIs enable quick frontend development without a backend dependency.

## Contributing

Contributions are welcome. If you plan to add features or refactor components:

1. Create a feature branch.
2. Keep changes focused and well-structured.
3. Run tests/build checks before opening a PR.
4. Provide clear PR descriptions and screenshots for UI-impacting changes.

## License

This project currently has no explicit license file. Add a `LICENSE` if you want to define usage terms.
