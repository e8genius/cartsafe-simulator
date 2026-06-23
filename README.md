# CartSafe Storefront Checkout Simulator

This repository contains the **Storefront Checkout Simulator** for **CartSafe** — a native Shopify application designed to protect merchant margins from double-discounting exploits (specifically stacking promotional coupon codes with gift cards).

The simulator is a Next.js application that mimics an e-commerce checkout page. It is used to test and demonstrate the functionality of CartSafe's safety net layers (Frontend Deterrent and Thank You Banner) without requiring a live, full Shopify store setup.

---

## 📁 Repository Structure

- `src/app/` - Storefront pages, cart, checkout, payment, thank-you pages, and admin controls.
- `src/components/` - Express checkout modal, header, and the CartSafe banner notification.
- `docs/` - A copy of the complete CartSafe product documentation.

---

## 🔗 Related Repositories

This simulator is part of the larger CartSafe project:
- **Shopify App & Analysis Repo:** [cartsafe-poc](https://github.com/e8genius/cartsafe-poc) — contains the core Shopify App codebase, background webhooks, PostgreSQL models, and the initial market research.

---

## 🛠️ Technical Stack

- **Framework:** Next.js 16 (App Router)
- **Styling:** Tailwind CSS v4
- **Components & Icons:** React, Lucide React

---

## 🔧 Local Development Quickstart

Follow these steps to set up and run the simulator locally:

### 1. Install Dependencies
```bash
npm install
```

### 2. Launch the Development Server
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser to view the storefront checkout simulator.

### 3. Testing Stacking Logic
- Use the **Admin panel** in the simulator (or go to `/admin`) to configure active coupons and simulated store properties.
- Try checkout flows to see how the Checkout UI Extensions block double discounting when a user attempts to combine a promotion coupon and a gift card.

---

## 📚 Detailed Documentation

The complete project documentation is duplicated here under the `docs/` folder:
- **Product Requirements (PRD):** [PRD.md](docs/PRD.md)
- **Product positioning & FAQs:** [PR_FAQ.md](docs/PR_FAQ.md)
- **Technical Architecture:** [ARCHITECTURE.md](docs/ARCHITECTURE.md)
- **API & GraphQL Schema:** [API_FLOWS.md](docs/API_FLOWS.md)
- **Database Schema & Metafields:** [DATA_MODEL.md](docs/DATA_MODEL.md)
- **Security & Privacy:** [SECURITY.md](docs/SECURITY.md)
- **Testing Scenarios:** [TESTING_SCENARIOS.md](docs/TESTING_SCENARIOS.md)
- **Developer Roadmap:** [ROADMAP.md](docs/ROADMAP.md)
