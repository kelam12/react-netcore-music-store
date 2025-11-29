# React .NET Core Music Store

A full-stack music store application built with React frontend and ASP.NET Core backend, featuring Redux state management and Entity Framework data persistence.

## Technology Stack

- **Frontend**: React with Redux for state management
- **Backend**: ASP.NET Core with Entity Framework
- **Database**: SQL Server with EF Core migrations
- **UI Framework**: Semantic UI React for component styling
- **Routing**: React Router DOM for client-side navigation

## Prerequisites

- .NET Core SDK
- Node.js and npm/yarn
- SQL Server (local or remote instance)

## Installation

### Frontend Dependencies

```bash
# State management and middleware
npm install redux react-redux redux-thunk --save

# Development tools
npm install redux-devtools-extension --save

# Routing
npm install react-router-dom --save

# UI Components
npm install semantic-ui-react semantic-ui-css --save

# Redux Logger for development
npm install redux-logger --save
```

### Backend Setup

The backend uses Entity Framework Core for database operations. Ensure your database connection string is properly configured in `appsettings.json`.

## Database Migrations

### Add New Migration

**Mac/Linux (CLI):**
```bash
dotnet ef migrations add <migrationName>
```

**Windows (Visual Studio Package Manager Console):**
```powershell
Add-Migration <migrationName>
```

### Update Database

**Mac/Linux (CLI):**
```bash
dotnet ef database update
```

**Windows (Visual Studio Package Manager Console):**
```powershell
Update-Database
```

## Development Features

- **Redux State Management**: Centralized state with Redux
- **Middleware Support**: Redux Thunk for async actions and Redux Logger for development debugging
- **Entity Framework**: ORM for database operations with code-first migrations
- **Semantic UI**: Pre-styled React components for consistent UI
- **Client-side Routing**: React Router for navigation without page reloads

## Project Structure

```
Backend/          ASP.NET Core API with Entity Framework
src/              React application with Redux setup
public/           Static assets and HTML template
```
