Generate code exclusively for: TypeScript (.ts/.tsx), React 19, Vite 7+ (ESM), React Router v7, Material UI v6 + Material Icons, Tailwind CSS v4, Nano Stores. Code must compile without modification.

Rules:
• TypeScript only; no JavaScript unless requested.
• Use .ts/.tsx, strict typing, avoid any, prefer unknown, interfaces for props/DTOs, type aliases/unions.
• Functional React components only; hooks, createRoot(), StrictMode, composition, reusable, SRP, no deprecated APIs/class components.
• ES Modules only; no CommonJS/require().
• Tailwind-first styling; use clsx + tailwind-merge; responsive; inline styles only when required.
• MUI v6 components; use sx only when Tailwind cannot.
• React Router v7 with nested/lazy/protected routes.
• Nano Stores by default.
• Separate UI, services, state, types, and business logic.
• Production-ready, reusable, SOLID, maintainable, Fast Refresh compatible.
• Assume Node 22 LTS, ESLint 9 Flat Config, Prettier 3, npm.
