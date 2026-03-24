# 🚀 Users & Posts API | NestJS + Prisma + Supabase

A modern, scalable, and production-ready backend API. This project demonstrates a **Senior Fullstack** approach to building modular systems with a focus on security, type safety, and efficient cloud orchestration.

---

## 🧱 Architectural Vision

As a Senior Developer, my goal was to implement an architecture that balances **Developer Experience (DX)** with **Enterprise-grade security**.

### 1. Modular NestJS Framework
The backend follows a strict **modular architecture**. Each domain (Users, Auth, Posts) is isolated, ensuring the codebase remains maintainable, testable, and follows **SOLID** principles as the application scales.

### 2. Data Persistence: Prisma + Supabase
* **Prisma ORM:** I implemented Prisma to provide a **Type-Safe** layer over the database, eliminating runtime errors and streamlining schema migrations.
* **Supabase (PostgreSQL):** I chose Supabase to leverage a high-performance, hosted PostgreSQL instance, reducing infrastructure overhead while maintaining full control over the data layer.

### 3. Identity & Security Strategy
* **Dual Authentication:** The system supports both **JWT** (Stateless) and **Google OAuth 2.0**. Delegating identity to Google reduces the attack surface and enhances user trust.
* **Advanced Guards:** Security is enforced via **NestJS Guards**. They act as a specialized middleware layer to verify token integrity and enforce **Role-Based Access Control (RBAC)**.
* **Data Integrity:** All entry points are protected by **DTOs** and `class-validator`, ensuring only sanitized data reaches the business logic.

---

## 📂 Module Overview

* **Auth Module:** Manages Passport strategies (JWT & Google), token signing, and secure login flows.
* **Users Module:** Handles user profiles, role management, and relational data mapping.
* **Posts Module:** Full CRUD operations with integrated access control (ensuring users only manage their own content).

---

## 📚 API Documentation (Swagger)

The API is fully documented and testable via Swagger UI:
👉 [**Live Swagger Documentation**](https://users-posts-api.up.railway.app/api)

---

## 🔐 Authentication Endpoints

| Strategy | Endpoint |
| :--- | :--- |
| **Google OAuth** | `https://users-posts-api.up.railway.app/auth/google` |
| **Local JWT** | `https://users-posts-api.up.railway.app/auth/login` |

---

> **Senior Insight:** This stack (NestJS/Prisma/Supabase) was chosen to minimize **Time-to-Market** while providing a robust foundation that can easily transition from a MVP to a high-traffic production environment.

---

**Would you like me to help you write a "Local Development" section with the necessary `.env` variables to help others run your project?**
