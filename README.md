# Friday Night Football ⚽

## Introduction

Hello there! Welcome to the repository for Friday Night Football, a web application that started as an excuse to explore modern technologies like [Astro](https://astro.build/), [Strapi](https://strapi.io/), [Nx](https://nx.dev/) and build an app that helps friends organize and keep track of football matches.

The project's main focus is to build an application that helps friends keep track of matches played while determining the team for the next match based on players' rankings.

## Features

- Create and manage football matches 🗓️
- Record match results ⚽
- Automatically update player rankings based on match outcomes 📈
- View upcoming matches and team compositions 📋

## Prerequisites

Before setting up the project, ensure you have the following installed:

- Node.js (v16 or higher) and NPM
- Python (Strapi SQLite database)
- nx (optional)

## Instalation Instructions

To install Friday Night Football project, follow these steps:

1. Clone the repository:
   ```sh
   git clone https://github.com/surreira/friday-night-football
   ```
1. Change directory to project root:
   ```sh
   cd friday-night-football
   ```
1. Install project dependencies:
   ```sh
   npm install
   ```

## Project Setup

Before starting the application, you need to set up the frontend and backend environments.

### Astro Frontend

1. Change directory to the frontend app:
   ```sh
   cd apps/frontend
   ```
1. Create a `.env` file and set the required environment variables:
   ```sh
   # Sample .env file - Replace these values with your configuration
   STRAPI_API_URL=http://localhost:3000
   ```

### Strapi Backend

1. Change directory to the backend app:
   ```sh
   cd apps/backend
   ```
1. Create a `.env` file and set the required environment variables:
   ```sh
   # Sample .env file - Replace these values with your configuration
   HOST=0.0.0.0
   PORT=1337
   APP_KEYS="toBeModified1,toBeModified2"
   API_TOKEN_SALT=tobemodified
   ADMIN_JWT_SECRET=tobemodified
   JWT_SECRET=tobemodified
   ```
1. Install Strapi globally (if you haven't already, optional):
   ```sh
   npm install -g strapi
   ```
1. Install Strapi dependencies:
   ```sh
   npm install
   ```

## Development

To start the development environment, you will need to run both the frontend and backend apps.

### Frontend Development

```sh
cd apps/frontend
npm run dev
```

The frontend will be accessible at `http://localhost:3000`.

### Backend Development

```sh
cd apps/backend
npm run develop
```

The Strapi backend will be accessible at `http://localhost:1337`.

When developing the FNF plugin frontend admin UI also use the `watch-admin` command.

```sh
cd apps/backend
npm run strapi watch-admin
```

The live updating app will be accessible at `http://localhost:8000`.

## Deployment

[tbd]
