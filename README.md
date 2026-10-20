# MisToy · Backend

REST API and WebSocket server for MisToy.
Frontend: [mistoy-frontend](https://github.com/yahavmor/mistoy-frontend)

## Features

- Toys: CRUD with filtering and sorting, plus messages per toy
- Auth: signup, login and logout with sessions (express-session) and bcrypt-hashed passwords
- Users and reviews APIs, with admin-only actions protected by middleware
- Socket.io: a chat room per toy with typing indicators, and live shop updates for admins
- Logger service and request logging middleware

## Tech

Node.js, Express, MongoDB (native driver), Socket.io, express-session, bcrypt and cookie-parser.

## Run locally

```bash
cp .env.example .env   # add your MongoDB connection string
npm install
npm run dev
```

In development the server uses a local MongoDB (`mongodb://127.0.0.1:27017`). In production it reads `MONGO_URI` and `DB_NAME` from the environment.

---

Built by **Yahav Mor** · [Portfolio](https://yahavmor.github.io) · [LinkedIn](https://www.linkedin.com/in/yahav-mor-566291270/) · [GitHub](https://github.com/yahavmor)
