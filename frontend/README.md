# Task Manager Frontend

A modern task management application built with React, Tailwind CSS, and Vite.

## Features

- User authentication (login/register)
- Task management (create, read, update, delete)
- Task status tracking
- Dashboard with task statistics
- Responsive design
- Protected routes

## Tech Stack

- React
- React Router DOM
- Tailwind CSS
- Headless UI
- Heroicons
- Axios
- React Hot Toast

## Getting Started

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

3. Build for production:
```bash
npm run build
```

## Environment Setup

Make sure your backend API is running on port 5000. The frontend development server will proxy all `/api` requests to `http://localhost:5000`.

## Project Structure

```
src/
  ├── components/      # Reusable components
  ├── contexts/        # React contexts
  ├── hooks/           # Custom hooks
  ├── pages/           # Page components
  ├── App.jsx          # Main application component
  ├── main.jsx         # Application entry point
  └── index.css        # Global styles and Tailwind CSS
```

## Authentication

The application uses JWT tokens for authentication. Tokens are stored in localStorage and automatically included in API requests using axios interceptors.

## API Integration

All API requests are made using axios. The base URL is configured to use the development server's proxy setting for `/api` requests.

## Styling

The application uses Tailwind CSS for styling with custom components defined in `index.css`. The primary color scheme and other theme customizations are defined in `tailwind.config.js`.