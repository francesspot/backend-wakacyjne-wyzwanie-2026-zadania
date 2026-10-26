[Polski](README.md) | **English**

# Backend Track Tasks — Summer Challenge 2026

<p align="center">
  <img src="https://github.com/user-attachments/assets/7c32ec09-c2ac-4961-82e6-a98f04220510"/>
</p>

This repository is where we complete the tasks from the backend course of the **Solvro** student research group's Summer Challenge (*Wakacyjne Wyzwanie*). The course materials are in [backend-wakacyjne-wyzwanie-2026](https://github.com/Solvro/backend-wakacyjne-wyzwanie-2026).

## My solutions

Each task is on its own branch; the `main` branch contains only this description.

| Branch | Task | What was done |
|--------|------|---------------|
| [`franciszek-pora-0`](../../tree/franciszek-pora-0) | 0 — TypeScript warm-up | A Node.js script that writes "Elo żelo" to a file as many times as the current minute |
| [`franciszek-pora-1`](../../tree/franciszek-pora-1) | 1 — First NestJS app | Project setup, a sample endpoint and `GET /brewCoffee`, which returns HTTP **418 I'm a teapot** |
| [`franciszek-pora-2`](../../tree/franciszek-pora-2) | 2 — Database | PostgreSQL + **Prisma**: an ERD diagram (`diagram_ERD.png` with a description), a schema with trips, expenses (PLN/EUR/USD) and participants, a migration and a seed script |
| [`franciszek-pora-3`](../../tree/franciszek-pora-3) | 3 — REST API | CRUD modules for **trips**, **expenses** and **participants** (controllers, services, DTOs) |
| [`franciszek-pora-4`](../../tree/franciszek-pora-4) | 4 — Authentication | A `User` model, `POST /auth/register` and `POST /auth/login` with **bcrypt** password hashing and **JWT** (Passport), plus a JWT guard on the trip, expense, participant and user endpoints |

Tech stack: **NestJS**, **TypeScript**, **Prisma**, **PostgreSQL**.

## Running a task

```bash
git checkout franciszek-pora-4
npm install
npx prisma migrate dev     # requires a PostgreSQL database configured in .env
npm run start:dev
```
