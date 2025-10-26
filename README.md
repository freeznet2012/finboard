# Finboard
Personal Finance Dashboard

## Project Structure

This repository contains two main components:

### Angular Application (`angular-app/`)
The frontend application built with Angular, designed to be hosted on Vercel.

- **Framework**: Angular 17
- **Hosting**: Vercel
- **Features**: Modern web application for personal finance tracking

See [angular-app/README.md](./angular-app/README.md) for more details.

### Supabase Backend (`supabase/`)
The backend configuration using Supabase for database and serverless functions.

- **Database**: PostgreSQL (via Supabase)
- **Functions**: Supabase Edge Functions (Deno-based serverless)
- **Auth**: Supabase Authentication
- **Storage**: Database migrations and seed data

See [supabase/README.md](./supabase/README.md) for more details.

## Getting Started

1. **Frontend Development**:
   ```bash
   cd angular-app
   npm install
   npm start
   ```

2. **Backend Development**:
   ```bash
   cd supabase
   supabase start
   ```

## Deployment

- **Frontend**: Deploy to Vercel using the configuration in `angular-app/vercel.json`
- **Backend**: Managed through Supabase CLI and hosted on Supabase platform
