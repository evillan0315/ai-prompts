Here's the updated version of your AI coding instructions with **Vite 7** as the baseline and a few modernizations for your current stack.

---

# AI Coding Instructions

## Primary Technology Stack

Generate code exclusively for:

* TypeScript (.ts/.tsx)
* React 19
* Vite 7+ (ESM)
* Material UI v6
* Material Icons
* Tailwind CSS v4

Everything must be immediately compatible with a **Vite 7 + React 19 + TypeScript + Material UI v6 + Tailwind CSS v4** project.

---

# General Rules

## Language

* Use TypeScript only.
* Never generate JavaScript unless explicitly requested.
* Enable strict typing.
* Avoid `any`.
* Prefer `unknown` with proper type narrowing.
* Use interfaces for props, DTOs, and API models.
* Use discriminated unions where appropriate.
* Prefer `type` aliases for unions, intersections, and utility types.
* Export reusable types from dedicated `types` modules.

---

# React Standards

Always use:

* Functional components
* Hooks
* React 19 APIs
* StrictMode
* createRoot
* Composition over inheritance
* Small reusable components
* Single Responsibility Principle

Prefer:

* Custom hooks
* Context only when appropriate
* Lazy-loaded routes
* Suspense
* Error boundaries

Never use:

* Class components
* Deprecated lifecycle APIs
* Legacy Context API

---

# Vite Standards

Assume:

* Vite 7+
* ES Modules only
* Native ESM imports
* `import.meta`
* `import.meta.env`
* Fast Refresh
* Modern browser targets
* Standard Vite project structure

Avoid:

* CommonJS
* require()
* Legacy bundler patterns

---

# Material UI

Use:

* Material UI v6
* Material Icons
* Theme-aware components
* Responsive layouts
* Accessible components

Prefer:

* Box
* Stack
* Grid2
* Paper
* Card
* Typography
* Button
* IconButton
* Tooltip
* Menu
* Dialog
* Drawer

Use `sx` only when Tailwind cannot express the styling cleanly.

---

# Tailwind CSS

Use Tailwind CSS v4.

Rules:

* Utility-first styling
* Mobile-first responsive design
* Avoid inline styles unless dynamically required
* Use `clsx`
* Use `tailwind-merge` for conditional utilities
* Keep utility ordering consistent

Avoid unnecessary CSS modules unless specifically requested.

---

# Code Quality

Always produce code that is:

* Production-ready
* Strictly typed
* Readable
* Maintainable
* Modular
* Reusable
* Self-documenting
* Minimal duplication

Follow SOLID principles where appropriate.

---

# Architecture

Prefer feature-based organization.

```text
src/
├── assets/
├── components/
├── features/
├── hooks/
├── layouts/
├── pages/
├── router/
├── services/
├── stores/
├── styles/
├── types/
├── utils/
└── main.tsx
```

Separate:

* UI
* Business logic
* API
* State
* Utilities
* Types

---

# State Management

Default preference:

* Nano Stores

Stores should be:

* Typed
* Modular
* Reactive
* Composable

Avoid unnecessary global state.

---

# Routing

Assume React Router v7.

Prefer:

* Data Router APIs
* Route handles
* Lazy routes
* Nested layouts
* Protected routes
* Route-level error boundaries

---

# API Layer

Use:

* Service abstraction
* Typed DTOs
* Fetch wrapper
* Authentication support
* Request cancellation
* Centralized error handling

Avoid placing API logic inside components.

---

# UI Design

Design should be:

* Modern
* Minimal
* Enterprise
* Spacious
* Responsive
* Accessible

Favor:

* Cards
* Tables
* Statistics
* Charts
* Sidebars
* Breadcrumbs
* Search
* Filters
* Empty states
* Skeleton loaders

---

# Component Design

Components should be:

* Small
* Reusable
* Generic where appropriate
* Strongly typed
* Composition-friendly

Avoid oversized components with mixed responsibilities.

---

# Forms

Prefer:

* Controlled components
* Reusable form fields
* Validation
* Clear error states
* Accessible labels

---

# Tables

Build reusable tables supporting:

* Pagination
* Sorting
* Filtering
* Searching
* Selection
* Empty states
* Loading states

---

# Icons

Use Material Icons.

Avoid emojis inside application UI.

---

# Styling

Priority:

1. Tailwind CSS
2. Material UI components
3. `sx` prop when necessary

Avoid unnecessary CSS files.

---

# Naming

Use descriptive names.

Examples:

```text
UserProfileCard
MembershipTable
DashboardStats
CompanionGrid
BookingCalendar
BookingSummaryCard
```

Avoid vague names such as:

```text
Component1
Helper
Temp
Utils2
```

---

# Performance

Use when beneficial:

* lazy()
* Suspense
* memo()
* useMemo()
* useCallback()

Avoid premature optimization.

---

# Error Handling

Always include:

* Loading states
* Error states
* Empty states
* Retry actions where appropriate

---

# Accessibility

Ensure:

* Semantic HTML
* Keyboard navigation
* Proper ARIA attributes
* Visible focus states
* Accessible dialogs and menus

---

# Folder Organization

Prefer:

```text
assets/
components/
features/
hooks/
layouts/
pages/
router/
services/
stores/
styles/
types/
utils/
```

---

# Backend Preferences

When generating backend code, prefer:

* Node.js
* TypeScript
* NestJS
* Fastify
* Prisma
* Redis
* BullMQ
* Swagger/OpenAPI
* DTO validation
* Microservice-ready architecture
* Clean Architecture where appropriate

---

# Code Generation Expectations

Generated code should:

* Compile without modification
* Be production-ready
* Include all necessary imports
* Follow modern React and TypeScript best practices
* Match the existing project architecture when continuing a codebase
* Avoid placeholders unless explicitly requested
* Minimize unnecessary comments while keeping complex logic understandable
* Preserve type safety throughout the implementation
* Favor reusable abstractions over duplicated logic
* Respect React Fast Refresh requirements (e.g., avoid exporting non-component utilities from component files)

---

# Default Assumptions

Unless instructed otherwise, assume:

* React 19
* Vite 7+
* TypeScript (strict mode)
* React Router v7
* Material UI v6
* Tailwind CSS v4
* Nano Stores for state management
* ESLint 9 (Flat Config)
* Prettier 3
* Node.js 22 LTS
* npm as the package manager
* Modern evergreen browsers with ES2022+ support

These assumptions should be the baseline for all generated code unless the project explicitly specifies a different stack.
