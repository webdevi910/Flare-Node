# FlareNode

Nodejs has become one of the most popular server-side frameworks for web developers. With its easy-to-use architecture and high-performance capabilities, developers are able to build efficient and scalable applications.

As a curious developer, I have decided to create my own NodeJS framework inspired by the likes of NestJS. This framework seeks to provide a seamless experience for developers by simplifying commonly-tedious tasks and providing pre-built tools, ultimately allowing developers to be more productive and efficient.

Through this experiment, I seek to gain a deeper understanding of how frameworks like NestJS are built, and to explore new possibilities in the world of NodeJS web development.

## Features
- Dependency Injection
- Middleware Support
- Modular Architecture
- Routing
- Exception Handling
- And much more!

## Setup

Clone the repository first, and then run `npm i` to install the dependencies.

Then create a copy of `.env.example` file using this command: `cp .env.example .env`.

Now you need to update the `.env` file and then run `npm start` to launch the app.

## Pre-built Endpoints

### User Registration

```bash
curl -X POST http://localhost:3000/auth/register \
  -d '{"email": "john@gmail.com", "fullname": "John Doe", "password": "secret1234"}' \
  -H "Content-Type: application/json"
```

### User Login

```bash
curl -v -X POST http://localhost:3000/auth/login \
  -d '{"email": "john@gmail.com", "password": "secret1234"}' \
  -H "Content-Type: application/json"
```

### Email Verification

```bash
curl -v -X POST http://localhost:3000/auth/send-verification-email \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer <token>"
```
