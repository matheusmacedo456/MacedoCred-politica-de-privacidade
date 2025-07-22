# MacedoCred Privacy Policy - Professional Web Application

## Overview

This is a professional full-stack web application built with React and Express that displays a comprehensive privacy policy page for "MacedoCred". The application features a modern, corporate design following LGPD (Lei Geral de Proteção de Dados) compliance standards for a Brazilian financial services company.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **Routing**: Wouter for lightweight client-side routing
- **State Management**: TanStack Query for server state management
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **UI Components**: Complete shadcn/ui component library (New York style)
- **Build Tool**: Vite for fast development and optimized production builds

### Backend Architecture  
- **Runtime**: Node.js with Express.js framework
- **Language**: TypeScript with ES modules
- **Database ORM**: Drizzle ORM configured for PostgreSQL
- **Session Management**: Prepared for PostgreSQL sessions with connect-pg-simple
- **Development Server**: TSX for TypeScript execution in development

### Database Strategy
- **Primary Database**: PostgreSQL (configured via DATABASE_URL environment variable)
- **ORM**: Drizzle with schema-first approach located in `shared/schema.ts`
- **Migrations**: Managed through drizzle-kit with output to `./migrations`
- **Current State**: Uses in-memory storage class as placeholder until database is connected

## Key Components

### Frontend Structure
- **Main App**: Single-page application with privacy policy focus
- **UI Library**: Complete shadcn/ui component set including forms, dialogs, navigation, and interactive elements
- **Pages**: Privacy policy page with smooth scrolling, mobile menu, and back-to-top functionality
- **Layout**: Responsive design with mobile-first approach and professional corporate styling

### Backend Structure
- **Express Server**: Minimal API structure with middleware for logging and error handling
- **Storage Interface**: Abstract storage pattern with in-memory implementation
- **Routes**: Placeholder structure for future API endpoints under `/api` prefix
- **Development Tools**: Vite integration for development with hot module replacement

### Styling System
- **Theme**: Professional blue and gold color scheme matching MacedoCred branding
- **Typography**: Google Fonts integration (Inter and Poppins)
- **Components**: CSS variables for consistent theming across all components
- **Responsiveness**: Mobile-first design with breakpoints for tablet and desktop

## Data Flow

### Current Implementation
1. Static content rendering for privacy policy
2. Client-side routing between pages
3. Responsive navigation with mobile menu toggle
4. Scroll behavior management for user experience

### Database Ready Architecture
1. User schema defined with Drizzle ORM (id, username, password)
2. Storage interface ready for CRUD operations
3. Session management prepared for PostgreSQL
4. Migration system configured for schema changes

## External Dependencies

### Core Dependencies
- **@neondatabase/serverless**: PostgreSQL database connection
- **drizzle-orm**: Type-safe ORM for database operations  
- **@tanstack/react-query**: Server state management
- **wouter**: Lightweight React router
- **date-fns**: Date manipulation utilities

### UI Dependencies
- **@radix-ui/***: Comprehensive set of accessible UI primitives
- **tailwindcss**: Utility-first CSS framework
- **lucide-react**: Modern icon library
- **class-variance-authority**: Component variant management

### Development Dependencies
- **vite**: Build tool and development server
- **typescript**: Type checking and compilation
- **tsx**: TypeScript execution for Node.js
- **esbuild**: Fast JavaScript bundler for production

## Deployment Strategy

### Build Process
1. **Frontend Build**: Vite compiles React app to `dist/public`
2. **Backend Build**: esbuild bundles server to `dist/index.js`
3. **Asset Optimization**: Automatic optimization of images and CSS

### Environment Configuration
- **Development**: `npm run dev` - TSX server with Vite HMR
- **Production**: `npm run build && npm start` - Optimized builds
- **Database**: Requires `DATABASE_URL` environment variable

### Production Requirements
- Node.js runtime for Express server
- PostgreSQL database connection
- Environment variables for database and session configuration
- Static file serving for built React application

### Replit Integration
- **Development Tools**: Runtime error overlay and cartographer for debugging
- **File Structure**: Organized for easy Replit deployment
- **Asset Management**: Attached assets folder for documentation and resources