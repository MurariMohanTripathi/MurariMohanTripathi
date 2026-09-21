<h1 align="center">Murari Mohan Tripathi</h1>

<p align="center">
  B.Tech (CSE) Graduate • Software Developer • Backend & Full-Stack Focus
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/murarimohantripathi/">LinkedIn</a> •
  <a href="https://muraritripathi.xyz">Portfolio</a> •
  <a href="mailto:tripathimurari599@gmail.com">Email</a> •
  <a href="https://leetcode.com/u/murarimohantripathi/">Leetcode</a>
</p>

---

## About

- Software developer with professional experience working on production applications and large existing codebases.
- Experienced in feature development, debugging, third-party integrations, payment workflows, booking flows, and database-driven modules.
- I enjoy building end-to-end products and backend services that solve practical business problems.
- Strong interest in backend development, full-stack engineering, system design fundamentals, APIs, payments, and scalable application architecture.

---

## Professional Experience

### Software Engineer Trainee — Webkul Software Pvt. Ltd., Noida

Working on **QloApps**, a hotel booking and property-management platform used for real-world hospitality workflows.

**Relevant Work**
- Developed and enhanced production features across booking, checkout, payment, membership, marketplace, email-template, and hotel-management workflows.
- Worked on third-party integrations and payment-related modules, including configuration, validation, transaction flows, and failure handling.
- Implemented and debugged business-critical booking flows involving carts, room reservations, extra services, order details, approvals, and customer actions.
- Worked on existing large codebases, traced issues across multiple modules, and delivered fixes while maintaining compatibility with current platform behaviour.
- Built and improved admin-side functionality, validations, status handling, configuration pages, and user-facing workflows.
- Worked with database-backed business logic, debugging incorrect data states and improving consistency between user actions, orders, payments, and booking records.
- Collaborated on production tasks that required understanding existing architecture before implementing changes safely.

---

## Projects

### PhonePe Payment Service — Centralized Payment Backend

A reusable payment service designed to act as a central payment layer for multiple applications while keeping payment processing, verification, status tracking, and provider communication outside the client application.

**Key Features**
- Creates PhonePe checkout orders through a dedicated payment API.
- Generates unique merchant order IDs for internal payment tracking.
- Stores payment records locally before and after provider communication.
- Maintains normalized payment states such as created, pending, completed, and failed.
- Provides a payment-status endpoint that checks the latest state from PhonePe and synchronizes it with the local payment record.
- Handles asynchronous PhonePe webhook events for completed and failed transactions.
- Verifies webhook authenticity using PhonePe-provided signature information before processing payment updates.
- Uses the original raw request payload where required for webhook signature verification.
- Separates payment creation, provider communication, webhook processing, persistence, and API handling into dedicated application layers.
- Designed so other projects can integrate with one payment service instead of implementing PhonePe logic repeatedly.
- Includes health and database connectivity checks for deployment and operational debugging.
- Supports sandbox and production-style environment separation through configuration.

**Payment Flow**
1. Client creates a payment request.
2. The service validates the request and creates a merchant order ID.
3. A local payment record is created.
4. The service creates the checkout order with PhonePe.
5. PhonePe returns the provider order information and checkout URL.
6. The local payment record is updated and the checkout URL is returned to the client.
7. The customer completes or fails the payment on PhonePe.
8. PhonePe sends an asynchronous webhook event.
9. The service verifies the webhook and updates the local payment state.
10. The client can independently request the latest payment status, which is reconciled with PhonePe before being returned.

**Links**  
GitHub: https://github.com/MurariMohanTripathi/PhonePe-Payment-Service  
Live API: https://phonepe-payment-service.onrender.com

---

### PortZen — Portfolio Builder for Developers

A customizable portfolio-building platform that allows developers to create and publish portfolios through their own public username-based URL.

**Key Features**
- Dynamic portfolio sections
- Multiple themes and pre-designed templates
- Public portfolio URL such as `portzen.in/username`
- Username availability checking
- Drag-and-drop section ordering
- Developer stories
- Custom code mode with sanitized HTML/CSS
- Basic analytics for views, visits, clicks, and bookmarks

**Links**  
GitHub: https://github.com/MurariMohanTripathi/portzen_frontend  
Live: https://portzen.in

---

### Verify — AI-Powered News Verification Platform

AI + community-driven system designed to validate news credibility and reduce misinformation.

**Key Features**
- AI-assisted news verification
- One User – One Vote model
- Spam and fake-content filtering during submission
- AI Verification Badge for trusted news
- Structured submission → validation → voting workflow
- Multiple UI themes

**Links**  
Frontend: https://github.com/MurariMohanTripathi/verify_frontend  
Backend: https://github.com/MurariMohanTripathi/verify_backend  
Live: https://verify-2db20.web.app/

---

### CampusCare — Complaint & Announcement System

A role-based college complaint and communication platform.

**Key Features**
- Student, Department Admin, and SuperAdmin dashboards
- Complaint submission and status tracking
- Announcement management
- Complaint inbox and administration workflow
- Role-based access control

Live: https://players-e502c.web.app/

---

### Blogify — Blogging Platform

A full blogging application focused on publishing, authentication, content management, and user interaction.

**Key Features**
- User authentication
- Blog creation and publishing
- Rich-text content editing
- Comments and user interaction
- Cloud deployment

Live: http://blogify-env.eba-5wpg9p66.ap-south-1.elasticbeanstalk.com/

---

### RevenueHub — Analytics Dashboard

An analytics-focused dashboard for presenting business and application metrics.

**Key Features**
- Data visualization
- Role-based dashboard rendering
- Responsive dashboard interface
- Structured presentation of business metrics

---

## Current Job Preference

I am currently looking for **entry-level / early-career Software Developer opportunities** where I can contribute to real production systems and continue growing as an engineer.

**Preferred Roles**
- Software Developer / Software Engineer
- Backend Developer
- Full-Stack Developer
- Associate Software Engineer
- SDE-1

**Preferred Locations**
- Noida
- Greater Noida
- Gurugram
- Delhi NCR
- Remote opportunities in India

I am particularly interested in roles involving **backend engineering, APIs, payments, business workflows, database-driven applications, integrations, and scalable product development**.

---

## GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=MurariMohanTripathi&show_icons=true" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=MurariMohanTripathi&layout=compact" />
</p>
