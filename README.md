# Astro + Strapi Blog Project

This is a modern blog application built with Astro 5 for the frontend and Strapi 5 for the backend CMS. The project demonstrates a full-stack application using these powerful technologies together.

## 🚀 Project Structure

The project is organized into two main directories:

```
├── client/           # Astro frontend application
│   ├── src/         # Source code for the frontend
│   ├── public/      # Static assets
│   └── .astro/      # Astro build output
│
├── server/          # Strapi backend application
│   ├── src/         # Source code for the backend
│   ├── config/      # Strapi configuration
│   ├── database/    # Database files
│   └── public/      # Public assets
│
└── resources/       # Additional project resources
```

## 🛠️ Tech Stack

### Frontend (Client)
- [Astro 5](https://astro.build/) - Modern static site builder
- [TailwindCSS](https://tailwindcss.com/) - Utility-first CSS framework
- [Strapi Client](https://docs.strapi.io/dev-docs/plugins/users-permissions) - Official Strapi client for frontend integration

### Backend (Server)
- [Strapi 5](https://strapi.io/) - Headless CMS
- TypeScript - For type-safe development
- SQLite (default) - Database (can be configured for other databases)

## 🏗️ Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (v18 or higher)
- Yarn package manager
- Git

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd strapi-blog
   ```

2. **Install dependencies and setup the project**
   ```bash
   yarn setup
   ```
   This command will:
   - Install root dependencies
   - Setup the client (frontend)
   - Setup the server (backend)
   - Copy necessary environment files

3. **Start the development servers**
   ```bash
   yarn dev
   ```
   This will start both the Strapi backend (port 1337) and Astro frontend (port 4321) concurrently.

## 📝 Available Scripts

- `yarn setup` - Initial project setup
- `yarn dev` - Start both frontend and backend in development mode
- `yarn client` - Run only the frontend development server
- `yarn server` - Run only the backend development server
- `yarn seed` - Import seed data into Strapi
- `yarn export` - Export Strapi data

## 🔧 Environment Setup

The project uses environment variables for configuration. The setup script will create the necessary `.env` files, but you may need to customize them:

### Client (.env)
- `PUBLIC_STRAPI_URL` - URL of your Strapi backend
- `PUBLIC_STRAPI_API_TOKEN` - API token for Strapi

### Server (.env)
- `HOST` - Host for Strapi server
- `PORT` - Port for Strapi server
- `APP_KEYS` - App keys for Strapi
- `API_TOKEN_SALT` - Salt for API tokens
- `ADMIN_JWT_SECRET` - JWT secret for admin panel
- `JWT_SECRET` - JWT secret for API
- `DATABASE_CLIENT` - Database client (default: sqlite)

## 📚 Learning Resources

- [Astro Documentation](https://docs.astro.build/)
- [Strapi Documentation](https://docs.strapi.io/)
- [TailwindCSS Documentation](https://tailwindcss.com/docs)

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- [Astro](https://astro.build/) for the amazing frontend framework
- [Strapi](https://strapi.io/) for the powerful headless CMS
- [TailwindCSS](https://tailwindcss.com/) for the utility-first CSS framework
