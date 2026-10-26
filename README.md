**Polski** | [English](README.en.md)

# Zadania ze ścieżki Backend — Wakacyjne Wyzwanie 2026

<p align="center">
  <img src="https://github.com/user-attachments/assets/7c32ec09-c2ac-4961-82e6-a98f04220510"/>
</p>

To repozytorium jest miejscem, w którym wykonujemy zadania z kursu backendowego Wakacyjnego Wyzwania koła naukowego **Solvro**. Materiały kursu znajdują się w repozytorium [backend-wakacyjne-wyzwanie-2026](https://github.com/Solvro/backend-wakacyjne-wyzwanie-2026).

## Moje rozwiązania

Każde zadanie jest na osobnej gałęzi; gałąź `main` zawiera tylko ten opis.

| Gałąź | Zadanie | Co zostało zrobione |
|-------|---------|---------------------|
| [`franciszek-pora-0`](../../tree/franciszek-pora-0) | 0 — rozgrzewka w TypeScripcie | Skrypt Node.js zapisujący do pliku „Elo żelo" tyle razy, ile wynosi bieżąca minuta |
| [`franciszek-pora-1`](../../tree/franciszek-pora-1) | 1 — pierwsza aplikacja w NestJS | Utworzenie projektu, przykładowy endpoint i `GET /brewCoffee`, który zwraca HTTP **418 I'm a teapot** |
| [`franciszek-pora-2`](../../tree/franciszek-pora-2) | 2 — baza danych | PostgreSQL + **Prisma**: diagram ERD (`diagram_ERD.png` z opisem), schemat z wycieczkami, wydatkami (PLN/EUR/USD) i uczestnikami, migracja i skrypt seedujący |
| [`franciszek-pora-3`](../../tree/franciszek-pora-3) | 3 — REST API | Moduły CRUD dla **wycieczek**, **wydatków** i **uczestników** (kontrolery, serwisy, DTO) |
| [`franciszek-pora-4`](../../tree/franciszek-pora-4) | 4 — uwierzytelnianie | Model `User`, `POST /auth/register` i `POST /auth/login` z hashowaniem haseł **bcrypt** i tokenami **JWT** (Passport) oraz guard JWT na endpointach wycieczek, wydatków, uczestników i użytkowników |

Technologie: **NestJS**, **TypeScript**, **Prisma**, **PostgreSQL**.

## Uruchomienie zadania

```bash
git checkout franciszek-pora-4
npm install
npx prisma migrate dev     # wymaga bazy PostgreSQL skonfigurowanej w .env
npm run start:dev
```
