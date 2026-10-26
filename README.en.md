🇵🇱 [Polski](README.md) | 🇬🇧 **English**

# ⚙️ NestJS Backend — Summer Challenge 2026

![NestJS](https://img.shields.io/badge/NestJS-E0234E?logo=nestjs&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white) ![Prisma](https://img.shields.io/badge/Prisma-2D3748?logo=prisma&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)

> 🎓 Backend track of the **Summer Challenge 2026** (*Wakacyjne Wyzwanie*) run by the **KN Solvro** student research group (Wrocław University of Science and Technology)

A REST API built step by step for **planning trips and splitting expenses** — from the first endpoint to JWT authentication. Each task lives on its own branch.

## 🪜 Steps

| # | Branch | What I did |
|---|---|---|
| 0 | [`franciszek-pora-0`](../../tree/franciszek-pora-0) | TypeScript and Node.js warm-up |
| 1 | [`franciszek-pora-1`](../../tree/franciszek-pora-1) | First NestJS app — including a `/brewCoffee` endpoint that returns **418 I'm a teapot** |
| 2 | [`franciszek-pora-2`](../../tree/franciszek-pora-2) | Database design (**ERD diagram**), **Prisma** schema: trips, expenses in PLN/EUR/USD, participants; migration and seed |
| 3 | [`franciszek-pora-3`](../../tree/franciszek-pora-3) | **CRUD** for trips, expenses and participants (controllers, services, DTOs) |
| 4 | [`franciszek-pora-4`](../../tree/franciszek-pora-4) | **Sign-up and login** — passwords hashed with **bcrypt**, **JWT** tokens (Passport) and a guard protecting the endpoints |

## 🚀 Run it

```bash
git checkout franciszek-pora-4
npm install
npx prisma migrate dev     # needs a PostgreSQL database in .env
npm run start:dev
```
