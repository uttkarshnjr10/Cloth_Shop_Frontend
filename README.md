# Anupriya Fashion Hub — Frontend

> **Where Tradition Meets Trend**
>
> A modern, responsive web application for managing a clothing shop — built for customers, staff, and owners.

---

## ✨ Features

### 🛍️ Customer Storefront

- Browse the product catalog with category filters and search
- View detailed product information in a slide-out drawer
- Responsive hero banner and product grid

### 👔 Staff Dashboard

- Record sales with multi-payment support (Cash / Online / Dues)
- Manage inventory — add, update, and track stock
- Track and manage customer dues
- View recent activity feed

### 👑 Owner Dashboard

- View sales history and analytics with interactive charts
- Monitor inventory history and stock changes
- Register and manage staff members
- Dashboard stats cards and sticky notes

### 🔐 Authentication

- Role-based login (Owner / Staff) with JWT authentication
- Automatic access-token refresh via interceptors
- Protected routes per role

---

## 🛠️ Tech Stack

| Layer         | Technology                                            |
| ------------- | ----------------------------------------------------- |
| Framework     | [React 18](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/) |
| Build Tool    | [Vite](https://vite.dev/)                             |
| Styling       | [Tailwind CSS](https://tailwindcss.com/) + [shadcn/ui](https://ui.shadcn.com/) |
| UI Components | [Radix UI](https://www.radix-ui.com/) · [Framer Motion](https://www.framer.com/motion/) · [Recharts](https://recharts.org/) |
| Routing       | [React Router v6](https://reactrouter.com/)           |
| State / Data  | [TanStack React Query](https://tanstack.com/query) · React Context |
| HTTP Client   | [Axios](https://axios-http.com/)                      |
| Forms         | [React Hook Form](https://react-hook-form.com/) + [Zod](https://zod.dev/) |
| Deployment    | [Vercel](https://vercel.com/)                         |

---

## 📁 Project Structure

```
src/
├── components/
│   ├── dashboard/      # Owner & Staff dashboard widgets
│   ├── layout/         # Sidebar, bottom nav
│   ├── shop/           # Storefront components
│   └── ui/             # shadcn/ui primitives
├── context/            # AuthContext (JWT auth state)
├── data/               # Mock / seed data
├── hooks/              # Custom React hooks
├── layout/             # ProtectedRoute wrapper
├── lib/                # Axios instance, utilities
├── pages/              # Route-level page components
└── main.tsx            # App entry point
```

---

## 🚀 Getting Started

### Prerequisites

- **Node.js** ≥ 18 — [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating)
- **npm** ≥ 9

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/uttkarshnjr10/Cloth_Shop_Frontend.git

# 2. Navigate into the project
cd Cloth_Shop_Frontend

# 3. Install dependencies
npm install

# 4. Start the development server
npm run dev
```

The app will be available at **http://localhost:5173**.

### Environment Variables

Create a `.env` file in the project root (see `.env.example` if available):

```
VITE_API_URL=https://your-api-domain.com/api/v1
```

---

## 📜 Available Scripts

| Command            | Description                          |
| ------------------ | ------------------------------------ |
| `npm run dev`      | Start the Vite dev server            |
| `npm run build`    | Production build                     |
| `npm run build:dev`| Development build                    |
| `npm run preview`  | Preview the production build locally |
| `npm run lint`     | Run ESLint                           |

---

## 🗺️ Route Map

| Path                  | Access   | Description                |
| --------------------- | -------- | -------------------------- |
| `/`                   | Public   | Landing page (role select) |
| `/shop`               | Public   | Customer storefront        |
| `/login`              | Public   | Login page                 |
| `/owner`              | Owner    | Owner dashboard            |
| `/owner/sales`        | Owner    | Sales history              |
| `/owner/inventory`    | Owner    | Inventory history          |
| `/staff`              | Staff    | Staff dashboard            |
| `/staff/billing`      | Staff    | Billing / record sales     |
| `/staff/inventory`    | Staff    | Inventory management       |
| `/staff/dues`         | Staff    | Dues management            |

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch — `git checkout -b feature/your-feature`
3. Commit your changes — `git commit -m "Add your feature"`
4. Push to the branch — `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📄 License

This project is private. All rights reserved.
