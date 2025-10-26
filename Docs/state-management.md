# State Management & Data Flow

## Approach
- Lightweight Angular Services + RxJS BehaviorSubjects / Signals  
- Shared services for cross-component updates  

## Example
```ts
@Injectable({ providedIn: 'root' })
export class HoldingsService {
  private holdings$ = new BehaviorSubject<Holding[]>([]);
  get holdings() { return this.holdings$.asObservable(); }
}
```

## Flow
1. Components subscribe to reactive streams.  
2. Any mutation triggers dashboard auto-refresh.  
3. Supabase SDK directly updates remote tables.  
4. Changes sync across tabs automatically.
