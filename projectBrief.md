# Roo Example Fullstack Project

This repository contains a fullstack application with a Django backend and Next.js frontend.

## Backend Architecture

The backend uses the Django framework with the following components:

- Django REST Framework for API development
- PostgreSQL database
- JWT authentication
- Celery for background tasks (optional)
- Django ORM for database operations
- Django Admin for administrative interface
- Follow the newest and most secure backend standards
- Implement Swagger/OpenAPI for API documentation

## Frontend Architecture

The frontend is built with:

- Next.js (newest version) with App Router
- TypeScript for type safety
- Zustand for state management
- NextAuth.js for authentication
- Tailwind CSS for styling (recommended)
- Axios for API requests
- Use OpenAPI code generator to generate SDK for the backend API
- ULTRA IMPORTANT: Always use the generated SDK to call the API - DO NOT implement API calls manually

## Project Structure

```
roo-example-fullstack/
├── backend/                # Django backend
│   ├── apps/               # Django apps
│   ├── config/             # Django settings
│   ├── manage.py           # Django management script
│   ├── requirements.txt    # Python dependencies
│   └── .env                # Environment variables
│
├── frontend/               # Next.js frontend
│   ├── app/                # Next.js App Router structure
│   ├── components/         # Reusable React components
│   ├── lib/                # Utility functions and custom hooks
│   ├── public/             # Static assets
│   ├── store/              # Zustand store definitions
│   └── package.json        # Node.js dependencies
│
├── docker-compose.yml      # Docker configuration
└── README.md               # Project documentation
```

## Getting Started

### Backend Setup

1. Navigate to the backend directory: `cd backend`
2. Create a virtual environment: `python -m venv venv`
3. Activate the virtual environment:
   - Windows: `venv\Scripts\activate`
   - Unix/MacOS: `source venv/bin/activate`
4. Install dependencies: `pip install -r requirements.txt`
5. Run migrations: `python manage.py migrate`
6. Start the development server: `python manage.py runserver`

### Frontend Setup

1. Navigate to the frontend directory: `cd frontend`
2. Install dependencies: `npm install`
3. Create a `.env.local` file for environment variables
4. Start the development server: `npm run dev`

## Development Workflow

1. Backend development uses Django CLI for creating apps, models, and running migrations
2. Frontend development follows Next.js conventions with App Router
3. State management is handled with Zustand stores
4. Authentication is implemented using NextAuth.js on the frontend and JWT on the backend
