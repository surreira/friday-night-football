# Friday Night Football Backend

## Project Setup

Before starting the application, you need to set up the backend environment.

1. Change directory to the backend app:
   ```bash
   cd apps/backend
   ```
1. Create a `.env` file and set the required environment variables:
   ```bash
   # Sample .env file - Replace these values with your configuration
   HOST=0.0.0.0
   PORT=1337
   APP_KEYS="toBeModified1,toBeModified2"
   API_TOKEN_SALT=tobemodified
   ADMIN_JWT_SECRET=tobemodified
   JWT_SECRET=tobemodified
   ```
1. Install Strapi globally (if you haven't already, optional):
   ```bash
   npm install -g strapi
   ```
1. Install Strapi dependencies:
   ```bash
   npm install
   ```

## Development

To start the development environment, you will need to run backend app.

```bash
cd apps/backend
npm run develop
```

The Strapi backend will be accessible at `http://localhost:1337`.
