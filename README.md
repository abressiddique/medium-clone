# Medium Project

This project is a full-stack application that demonstrates the integration of various technologies. It consists of a backend service, a shared common utility package, and a frontend interface.

## Project Structure

- **Backend**: Implements API services and data handling using Hono, Prisma, and Cloudflare Workers.
- **Common**: A shared utility package with common types and functions used across the backend and frontend.
- **Frontend**: A web interface built with React, Vite, and Tailwind CSS.

## Backend

The backend is built with Cloudflare Workers and Hono for handling HTTP requests and Prisma for database interactions.

### Scripts

- `dev`: `wrangler dev src/index.ts` - Runs the backend locally.
- `deploy`: `wrangler deploy --minify src/index.ts` - Deploys the backend to Cloudflare Workers.

### Dependencies

- `@abres/medium-common`: Shared utilities.
- `@prisma/client`: Prisma client for database access.
- `@prisma/extension-accelerate`: Prisma extension for performance optimization.
- `hono`: A lightweight framework for building HTTP APIs.
- `prisma`: Prisma ORM for managing database schemas.

### Dev Dependencies

- `@cloudflare/workers-types`: TypeScript definitions for Cloudflare Workers.
- `wrangler`: CLI tool for managing Cloudflare Workers.

## Common

The common package contains shared utilities and types used by both the backend and frontend.

### Dependencies

- `zod`: A TypeScript-first schema declaration and validation library.

## Frontend

The frontend is developed with React, Vite, and Tailwind CSS, providing a responsive and interactive user interface.

### Scripts

- `dev`: `vite` - Starts the development server.
- `build`: `tsc && vite build` - Compiles TypeScript and builds the project.
- `lint`: `eslint . --ext ts,tsx --report-unused-disable-directives --max-warnings 0` - Runs ESLint for code quality checks.
- `preview`: `vite preview` - Previews the production build.

### Dependencies

- `@abres/medium-common`: Shared utilities.
- `axios`: HTTP client for making requests.
- `react`: UI library for building user interfaces.
- `react-dom`: React package for DOM interactions.
- `react-router-dom`: Routing library for React.

### Dev Dependencies

- `@types/react`: TypeScript types for React.
- `@types/react-dom`: TypeScript types for React DOM.
- `@typescript-eslint/eslint-plugin`: ESLint plugin for TypeScript.
- `@typescript-eslint/parser`: ESLint parser for TypeScript.
- `@vitejs/plugin-react`: Vite plugin for React.
- `autoprefixer`: PostCSS plugin for adding vendor prefixes.
- `eslint`: Linter for JavaScript and TypeScript.
- `eslint-plugin-react-hooks`: ESLint plugin for React hooks.
- `eslint-plugin-react-refresh`: ESLint plugin for React refresh.
- `postcss`: Tool for transforming CSS with JavaScript.
- `tailwindcss`: Utility-first CSS framework.
- `typescript`: TypeScript compiler.
- `vite`: Build tool for modern web projects.

## Project Screenshots

Here is a screenshot of the project:

![Screenshot](demo/image.png)

## Getting Started

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
