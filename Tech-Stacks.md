# 1. Frontend Development

- Next.js: React framework for high-performance SSR, SSG, and unified routing/API handling.
- TanStack Query: Essential library for server state management (Query) and complex data UI (Table).
- Zod: TypeScript-first schema validation for runtime type safety in forms and APIs.
- Modernize Template: A pre-built UI foundation for rapid dashboard and landing page development.
- shadcn/ui: Accessible, customizable component primitives built with Radix UI and Tailwind CSS.
- Iconify-icons: A unified framework providing access to thousands of icons across multiple sets.
- lucide-react: A library of clean, consistent SVG icons designed for modern React interfaces.

## 2.1 Security and Authentication

- Supabase Client (@supabase/supabase-js): Primary authentication and data access layer. Handles JWT validation, Realtime subscriptions, and Storage access with Row-Level Security (RLS) enforcement.
- Next.js Middleware (proxy.ts): Server-side logic to intercept requests for edge-case routing and auth guards.
- Lark OAuth: Enterprise SSO protocol for secure user login via the Lark ecosystem. OAuth flow generates Supabase JWT tokens.
- NextAuth (Optional): Session management wrapper around Supabase JWT. Only needed if you want additional session helpers beyond direct Supabase JWT usage.

## 2.2 Authorization

- Supabase Row-Level Security (RLS): Database-level authorization policies that enforce access control at the data layer. Handles "who can see what data" automatically.
- CASL (Optional): UI-level authorization library for conditional rendering based on user abilities. Only needed if you require client-side ability checks beyond what RLS provides.

## 2.3 State Management

- TanStack Query: Server state management (caching, synchronization, optimistic updates).
- Zustand: Lightweight state management for client-side UI state (theme, sidebar, form drafts). 
  **Note:** When using Zustand with `persist` middleware for localStorage, implement client-only 
  hydration patterns (useEffect guards or dynamic imports) to prevent hydration mismatches.

## 2.4 Integration and Enterprise Tools

- Lark JS SDK: Utilize the built-in native features provided by Lark like geofencing and camera.

## 2.5 Development and Supporting Tools
- next-devtools-mcp: ability to enhance AI-assisted development, allowing for faster debugging and performance optimization.