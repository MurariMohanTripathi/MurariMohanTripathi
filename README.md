<h1 align="center">Murari Mohan Tripathi</h1>

<p align="center">
  <b>Software Developer • Backend Engineering • APIs • Payments • Business Systems</b>
</p>

<p align="center">
  I build backend systems around real business workflows — authentication, payments, orders, integrations, persistence, validation, and reliable state transitions.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/murarimohantripathi/">LinkedIn</a> •
  <a href="https://portzen.in/muraritripathi">Portfolio</a> •
  <a href="mailto:tripathimurari599@gmail.com">Email</a> •
  <a href="https://leetcode.com/u/murarimohantripathi/">LeetCode</a>
</p>

---

## 👨‍💻 About Me

I am a B.Tech (CSE) graduate and software developer with professional experience working on production applications, large existing codebases, business-critical workflows, third-party integrations, database-backed modules, and debugging.

I am most interested in the parts of software that sit behind the UI: **API design, authentication and authorization, payments, webhooks, order and booking flows, database consistency, integrations, validation, failure handling, and application architecture**.

I enjoy understanding how a system behaves end-to-end — from an incoming request, through business rules and persistence, to external services and the final state stored in the application.

---

## ⚙️ Backend Engineering Focus

- Designing REST-style APIs around real product workflows
- Authentication, authorization, role-based access, and protected resources
- Payment creation, provider communication, webhook handling, and payment-state synchronization
- Database-backed business logic and maintaining consistent application state
- Order, cart, checkout, booking, and transaction workflows
- Input validation, failure handling, edge cases, and debugging
- Third-party API integrations and asynchronous provider callbacks
- Working safely inside large existing codebases
- Separating routing, controllers, services, repositories, and persistence concerns
- Building reusable backend services that can support more than one client application

---

## 💼 Professional Experience

### Associate Software Engineer — Webkul Software Pvt. Ltd., Noida             [feb,2026 - sept,2026]

Working on **QloApps**, a production hotel booking and property-management platform with complex booking, checkout, payment, room, order, customer, and admin workflows.

**Backend-relevant work includes:**

- Developed and enhanced production features across booking, checkout, payments, memberships, marketplace flows, hotel operations, and customer workflows.
- Worked with third-party integrations and payment modules involving configuration, request validation, transaction flows, callbacks, and failure scenarios.
- Implemented and debugged business logic involving carts, room reservations, booking requests, extra services, order details, approvals, and payment transitions.
- Investigated issues across multiple modules and database-backed flows to identify incorrect application states and deliver compatible fixes.
- Worked on admin-side workflows involving configuration, status management, validations, and operational controls.
- Handled features where correctness depended on keeping customer actions, booking records, carts, orders, and payment states consistent.
- Regularly worked inside a large existing codebase where changes required understanding the surrounding architecture before implementation.

---

# 🚀 Selected Backend Projects

## 💳 PhonePe Payment Service — Centralized Payment Backend

A reusable payment service built to keep payment processing outside individual client applications and provide a single backend layer for payment creation, persistence, verification, webhook processing, and status reconciliation.

### What it handles

- Creates checkout payments through a dedicated API.
- Generates internal merchant order identifiers for transaction tracking.
- Persists payment information before and after provider communication.
- Maintains normalized transaction states such as created, pending, completed, and failed.
- Exposes an endpoint that retrieves the latest provider status and synchronizes the local payment record.
- Processes asynchronous payment-completed and payment-failed webhook events.
- Verifies webhook authenticity before accepting state-changing events.
- Preserves the raw webhook request where required for signature validation.
- Separates API handling, provider communication, webhook processing, and persistence responsibilities.
- Includes service-health and database-connectivity endpoints for operational debugging.
- Is designed as a reusable payment layer so multiple applications can integrate without reimplementing provider logic.

### Payment lifecycle

```text
Client
  │
  │ Create Payment
  ▼
Payment API
  │
  ├── Validate Request
  ├── Generate Merchant Order ID
  ├── Persist Initial Transaction
  │
  ▼
PhonePe Checkout
  │
  ├── Provider Order
  └── Redirect URL
  │
  ▼
Customer Payment
  │
  ▼
PhonePe Webhook
  │
  ├── Verify Authenticity
  └── Update Transaction State
  │
  ▼
Persisted Payment State
```

**Repository:** https://github.com/MurariMohanTripathi/PhonePe-Payment-Service  
**Live API:** https://phonepe-payment-service.onrender.com

---

## 🛒 MiniShop — E-Commerce Backend API

An e-commerce backend centered around authenticated users, role-protected operations, products, carts, inventory validation, checkout, and order history.

### Backend capabilities

- User registration and login with secure password hashing.
- JWT-based authentication with identity and role claims.
- Customer and Admin roles with authorization rules at API level.
- Protected cart endpoints scoped to the authenticated user.
- Product and category management with admin-only write operations.
- Inventory checks when products are added to or updated inside a cart.
- Checkout workflow that validates stock before creating an order.
- Captures product name, price, quantity, and totals into order records at checkout time.
- Reduces product inventory after successful order creation.
- Clears purchased cart items after checkout.
- Provides authenticated order-history and individual-order endpoints.
- Prevents users from accessing another user's cart or order data.

### Request flow

```text
Login
  │
  ▼
JWT
  │
  ▼
Protected API
  │
  ├── Products / Categories
  ├── Cart
  └── Orders
        │
        ├── Validate Ownership
        ├── Validate Inventory
        ├── Create Order
        ├── Update Stock
        └── Persist Result
```

**Repository:** https://github.com/MurariMohanTripathi/MiniShop

---

## 🧠 Verify — AI-Assisted News Verification Platform

A full product with a dedicated backend responsible for accepting content, supporting verification workflows, and serving the application's data and business processes.

**Backend-oriented highlights**

- API-backed application architecture with a dedicated backend repository.
- Structured submission and validation workflow.
- User-driven credibility signals with controlled voting behavior.
- AI-assisted verification integrated into the application flow.
- Content filtering and validation before information enters the main feed.
- Designed around multiple application states rather than a static AI response.

**Backend:** https://github.com/MurariMohanTripathi/verify_backend  
**Frontend:** https://github.com/MurariMohanTripathi/verify_frontend  
**Live:** https://verify-2db20.web.app/

---

## 🌐 PortZen — Developer Portfolio Platform

A multi-user portfolio platform where developers can build and publish their own customizable portfolio under a username-based public URL.

**Engineering highlights**

- Username-based public routing and availability validation.
- User-owned portfolio data and configurable sections.
- Dynamic ordering of sections and customizable themes.
- Sanitized custom-code mode for user-provided HTML/CSS.
- Analytics model for views, visits, clicks, and bookmarks.
- Authentication-backed user workflows and persistent portfolio configuration.
- Admin-oriented platform functionality alongside public user pages.

**Repository:** https://github.com/MurariMohanTripathi/portzen  
**Live:** https://portzen.in

---

## 🏫 CampusCare — Role-Based Complaint & Announcement System

A workflow-driven application built around multiple user roles and controlled access to complaints and announcements.

- Student, Department Admin, and SuperAdmin roles
- Complaint submission and status lifecycle
- Administrative complaint handling
- Announcement publishing
- Role-based access control
- Persistent user and complaint records

**Repository:** https://github.com/MurariMohanTripathi/CampusCare  
**Live:** https://players-e502c.web.app/

---

## 🧩 How I Approach Backend Problems

When I build or debug a backend feature, I try to reason about the complete state transition rather than only the endpoint.

```text
Request
   ↓
Authentication / Authorization
   ↓
Validation
   ↓
Business Rules
   ↓
Database State
   ↓
External Integration (when needed)
   ↓
Failure / Success Handling
   ↓
Consistent Final State
   ↓
API Response
```

For payment, booking, checkout, and order workflows, I pay particular attention to **ownership, validation, failure paths, duplicate or asynchronous events, and keeping persisted state aligned with what actually happened**.

---

## 🎯 Current Job Preference

I am looking for **entry-level / early-career software engineering opportunities** where I can work on real production systems and continue developing depth in backend engineering.

**Roles of interest:** Backend Developer, Software Developer, Software Engineer, Full-Stack Developer, Associate Software Engineer, and SDE-1.

**Preferred locations:** Noida, Greater Noida, Gurugram, Delhi NCR, and remote opportunities in India.

I am especially interested in teams working on **APIs, payments, backend services, database-driven products, integrations, commerce, booking systems, authentication, and business-critical workflows**.

---

## 📊 GitHub Activity

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=MurariMohanTripathi&show_icons=true&hide_border=true" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=MurariMohanTripathi&layout=compact&hide_border=true" />
</p>
