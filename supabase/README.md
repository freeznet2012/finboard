# Finboard Supabase Configuration

This directory contains the Supabase backend configuration for Finboard.

## Structure

- `functions/` - Supabase Edge Functions
- `migrations/` - Database migration files
- `seed/` - Database seed data

## Getting Started

1. Install the Supabase CLI:
```bash
npm install -g supabase
```

2. Login to Supabase:
```bash
supabase login
```

3. Link to your project:
```bash
supabase link --project-ref your-project-ref
```

4. Start local development:
```bash
supabase start
```

## Database Migrations

Create a new migration:
```bash
supabase migration new migration_name
```

Apply migrations:
```bash
supabase db push
```

## Edge Functions

Create a new function:
```bash
supabase functions new function_name
```

Deploy functions:
```bash
supabase functions deploy function_name
```

## Environment Variables

Create a `.env` file in the root of your project with:
```
SUPABASE_URL=your-supabase-url
SUPABASE_ANON_KEY=your-anon-key
```
