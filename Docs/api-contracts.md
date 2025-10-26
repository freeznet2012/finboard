# API Contracts & Data Models

## Database Tables
- `users`, `categories`, `holdings`, `net_worth_history`, `user_settings`, `import_jobs`

## Key Models
```ts
export interface Category {
  id: string;
  user_id: string;
  name: string;
  type: 'asset' | 'liability';
  icon?: string;
  sort_order?: number;
  created_at?: string;
}

export interface Holding {
  id: string;
  user_id: string;
  category_id: string;
  type: 'asset' | 'liability';
  name: string;
  value: number;
  currency: string;
  notes?: string;
  last_updated?: string;
}
```

## CRUD Endpoints (via Supabase SDK)
- `getHoldings()`, `addHolding()`, `updateHolding()`, `deleteHolding()`  
- `getCategories()`, `addCategory()`, `updateCategory()`, `deleteCategory()`

## OpenAPI Snippet (for Edge)
```yaml
paths:
  /insights/snapshot:
    post:
      summary: Create net worth snapshot
      responses:
        '200':
          description: Snapshot saved
```
