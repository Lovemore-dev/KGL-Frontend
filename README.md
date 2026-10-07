# KGL Frontend

This is the frontend for Karibu Groceries Limited, a wholesale produce distribution management portal built with Vue 3 and Vite.

The application is designed to help the business manage operational workflows across procurement, sales, inventory, reporting, and user access from a single dashboard.

## What the project does

KGL Frontend provides a role-based business management system for the company:

- Landing page for the business and access entry points
- Secure login flow with role-based access control
- Executive dashboard for directors
- Branch operations dashboard for managers
- Sales tracking for sales agents
- Procurement management for incoming stock and supplier records
- Inventory visibility for stock levels and available produce
- Intelligence/reporting views for business performance
- User management for admin-level roles

## Main user roles

- Director: executive overview, company-level analytics, reporting, user management
- Manager: branch operations, stock monitoring, procurement and sales oversight
- Sales Agent: personal sales activity and sales record entry

## Tech stack

- Vue 3
- Vite
- Vue Router
- Pinia for state management
- Axios for API requests
- SweetAlert2 for alerts
- ESLint + Oxlint for linting

## Project structure

```text
src/
  App.vue
  main.js
  assets/
  router/
    index.js
  services/
    api.js
  stores/
    auth.js
  views/
    DashboardLayout.vue
    DashboardView.vue
    HomeView.vue
    IntelligenceView.vue
    InventoryView.vue
    LoginView.vue
    ProcurementView.vue
    SalesView.vue
    UserManagementView.vue
```

## Features implemented in the UI

- Role-aware route guards
- Dashboard cards with summary metrics
- Sales and procurement tables for operational tracking
- Inventory and stock visibility
- Business reporting and branch performance analytics
- Local user session handling using browser storage

## Getting started

### Install dependencies

```bash
npm install
```

### Run the app in development mode

```bash
npm run dev
```

### Build for production

```bash
npm run build
```

### Preview production build

```bash
npm run preview
```

### Lint the project

```bash
npm run lint
```

## Notes

- The app expects a backend service to provide business data for procurement, sales, inventory, and user information.
- Authentication state is currently maintained in local storage via the auth store.
- The project is structured around the KGL operations workflow rather than a generic starter template.

## Recommended development setup

- VS Code
- Vue extension support for editor tooling
- Browser devtools for frontend debugging
