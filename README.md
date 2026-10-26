🇵🇱 **Polski** | 🇬🇧 [English](README.en.md)

# ⚙️ Backend w NestJS — Wakacyjne Wyzwanie 2026

![NestJS](https://img.shields.io/badge/NestJS-E0234E?logo=nestjs&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white) ![Prisma](https://img.shields.io/badge/Prisma-2D3748?logo=prisma&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)

> 🎓 Ścieżka backendowa **Wakacyjnego Wyzwania 2026** koła naukowego **KN Solvro** (Politechnika Wrocławska)

Etapami zbudowane REST API do **planowania wycieczek i rozliczania wydatków** — od pierwszego endpointu po uwierzytelnianie JWT. Każde zadanie jest na osobnej gałęzi.

## 🪜 Etapy

| # | Gałąź | Co zrobiłem |
|---|---|---|
| 0 | [`franciszek-pora-0`](../../tree/franciszek-pora-0) | Rozgrzewka w TypeScripcie i Node.js |
| 1 | [`franciszek-pora-1`](../../tree/franciszek-pora-1) | Pierwsza aplikacja w NestJS — m.in. endpoint `/brewCoffee` zwracający **418 I'm a teapot** |
| 2 | [`franciszek-pora-2`](../../tree/franciszek-pora-2) | Projekt bazy (**diagram ERD**), schemat w **Prisma**: wycieczki, wydatki w PLN/EUR/USD, uczestnicy; migracja i seed |
| 3 | [`franciszek-pora-3`](../../tree/franciszek-pora-3) | **CRUD** dla wycieczek, wydatków i uczestników (kontrolery, serwisy, DTO) |
| 4 | [`franciszek-pora-4`](../../tree/franciszek-pora-4) | **Rejestracja i logowanie** — hasła w **bcrypt**, tokeny **JWT** (Passport) i guard chroniący endpointy |

## 🚀 Uruchomienie

```bash
git checkout franciszek-pora-4
npm install
npx prisma migrate dev     # potrzebna baza PostgreSQL w .env
npm run start:dev
```
