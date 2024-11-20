# Deadlock Content Server

A headless CMS powered by Strapi 5.4 that serves as the content management backend for the Deadlock Blog platform.

## Features

- Headless CMS with RESTful API and GraphQL endpoints
- User authentication and permissions management
- TypeScript support for enhanced type safety
- SQLite database for data storage
- Cloud-ready deployment configuration
- Custom API endpoints and content types
- Media library management

## Tech Stack

- **Framework**: Strapi 5.4.0
- **Language**: TypeScript 5
- **Database**: SQLite (better-sqlite3 11.3.0)
- **Runtime**: Node.js (>=18.0.0 <=22.x.x)
- **Authentication**: @strapi/plugin-users-permissions 5.4.0
- **Cloud Integration**: @strapi/plugin-cloud 5.4.0

## Prerequisites

- Node.js (>=18.0.0 <=22.x.x)
- npm (>=6.0.0)

## Getting Started

1. Clone the repository

2. Install dependencies:
```bash
npm install
```

3. Set up your environment variables:
   - Copy `.env.example` to `.env`
   - Configure your environment variables as shown below

4. Start the development server:
```bash
npm run develop
```

The admin panel will be available at: http://localhost:3001/admin

## Project Structure

```
deadlock-content-server/
├── config/         # Strapi configuration files
├── database/       # Database files and configurations
├── public/         # Static files
├── src/
│   ├── api/       # API definitions and controllers
│   ├── admin/     # Admin panel customizations
│   ├── extensions/  # Custom extensions and overrides
│   └── index.ts   # Main application entry point
└── types/         # TypeScript type definitions
```

## Available Scripts

- `npm run develop` - Start development server with auto-reload
- `npm run start` - Start production server
- `npm run build` - Build the admin panel
- `npm run strapi` - Access Strapi CLI
- `npm run deploy` - Deploy your Strapi application

## Environment Variables

Required environment variables for the application:

```
HOST=0.0.0.0
PORT=3001
APP_KEYS=your-app-keys
API_TOKEN_SALT=your-api-token-salt
ADMIN_JWT_SECRET=your-admin-jwt-secret
JWT_SECRET=your-jwt-secret
```

## API Documentation

Once the server is running, you can access:
- REST API documentation at: http://localhost:3001/documentation
- Admin panel at: http://localhost:3001/admin

---

## 📚 Strapi Documentation

For more information about using Strapi, please refer to the [official documentation](https://docs.strapi.io).
