# Coding Standards & Folder Structure

## Organization
Hybrid pattern:  
- Feature-based folders for major pages  
- Shared libs for UI, utils, and data-access

```
src/
├── app/
│   ├── features/
│   │   ├── dashboard/
│   │   ├── assets/
│   │   ├── liabilities/
│   │   ├── insights/
│   │   ├── categories/
│   ├── shared/
│   │   ├── ui/
│   │   ├── services/
│   │   ├── models/
│   │   ├── utils/
```

## Conventions
- Files: `kebab-case`  
- Classes: `PascalCase`  
- Variables/Functions: `camelCase`  

## Core Practices
✅ Dependency Injection  
✅ Central Logging Wrapper  
✅ Retry Policies (Exponential Backoff)  
✅ Strict TypeScript  
✅ DTO → Domain Mapper  
✅ Toast-based Error Handling  

## Tools
- ESLint (Angular preset)
- Husky + lint-staged pre-commit hooks
