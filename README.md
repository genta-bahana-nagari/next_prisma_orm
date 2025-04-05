# Next.js Prisma ORM Backend

This repository contains the **backend** of a web application built using **Next.js API routes** and **Prisma ORM**. It handles data management, authentication (optional), and RESTful or GraphQL APIs. This project does **not include any frontend views** — it is meant to function purely as a backend service.

## 🛠 Tech Stack

- **Next.js** – API routes used as serverless functions
- **Prisma ORM** – Type-safe database access
- **PostgreSQL** (or your DB of choicem you can use MySQL)
- **JavaScript**
- Optional: **JWT Auth**, **Zod validation**, **bcrypt**, etc.

---

## 📦 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/genta-bahana-nagari/next_prisma_orm.git
cd next_prisma_orm #or other directories if you renamed it.
```

### 2. Install Dependencies

```bash
npm install
# or
yarn install
```

### 3. Set Up Environment Variables

Create a `.env` file in the root of the project:

```env
DATABASE_URL="postgresql://user:password@localhost:5432/yourdb"
# Optional: JWT_SECRET, etc.
```
You can use 3306 port if you use MySQL

### 4. Set Up Prisma

Generate Prisma Client and run migrations:

```bash
npx prisma generate
npx prisma migrate dev --name init
```

### 5. Run the Development Server

```bash
npm run dev
# or
yarn dev
```

API will be available at: `http://localhost:3000/api`

---

## 📁 Project Structure

```
.
├── prisma/
│   └── schema.prisma      # Prisma schema definition
├── pages/
│   └── api/               # Next.js API routes
├── lib/                   # Utility functions and services
├── middleware/            # (Optional) Auth, logging, etc.
├── .env                   # Environment variables
├── package.json
└── README.md
```

---

## 🚀 Deployment

You can deploy this backend easily to:

- **Vercel** (recommended for serverless API routes)
- **Railway**, **Render**, or **Heroku**
- **Docker** (optional setup required)

If you want to deoloy it publicly, you can develop it with frontend page and make it more interactive.

---

## 🕪 Testing

Use your preferred testing application, such as Postman.

---

## 📝 Notes

- This repo is **backend-only** — no frontend components or UI are included.
- Intended to be used as a base or plug-in API layer for a full-stack app.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
