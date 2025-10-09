# 🚀 Next.js Starter Pack — Ready to Use Full-Stack Boilerplate

A **production-ready Next.js Starter Pack** with modern tools, pre-configured authentication, UI components, validation, and database integration — so you can **skip setup and start building right away**.

---

## ⚙️ Features

✅ **Next.js (App Router)** – Built with the latest Next.js architecture  
✅ **shadcn/ui** – Pre-configured and initialized for beautiful UI components  
✅ **NextAuth.js v5** – Fully configured authentication system  
- Credentials Provider (Email + Password)
- Google Sign-In ready
- Easily add more providers (GitHub, Apple, Facebook, etc.)

✅ **bcryptjs** – Secure password hashing  
✅ **Zod** – Type-safe schema validation  
✅ **React Hook Form** – Clean, declarative form handling  
✅ **Framer Motion** – Subtle, professional animations  
✅ **Prisma ORM** – Integrated with a PostgreSQL database  
✅ **Ready-to-use `schema.prisma`** – Predefined User model and Auth setup  
✅ **Full authentication flow** – Sign Up, Sign In, and Redirect  
✅ **Developer friendly** – Well-structured, extensible codebase

---

## 🧱 Tech Stack

| Tool | Purpose |
|------|----------|
| [Next.js](https://nextjs.org/) | React framework for full-stack apps |
| [shadcn/ui](https://ui.shadcn.com/) | Styled component library |
| [NextAuth.js v5](https://authjs.dev/) | Authentication |
| [bcryptjs](https://www.npmjs.com/package/bcryptjs) | Password hashing |
| [Zod](https://zod.dev/) | Schema validation |
| [React Hook Form](https://react-hook-form.com/) | Form management |
| [Framer Motion](https://www.framer.com/motion/) | Animations |
| [Prisma](https://www.prisma.io/) | ORM |
| [PostgreSQL](https://www.postgresql.org/) | Database |

---

## 🧰 Setup Instructions

### 1. Clone the repository
```terminal
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>

pnpm install
# or
npm install
# or
yarn install
```

### 2. Create .env file in root/src folder 

add these .env credentials

DATABASE_URL="postgresql://user:password@localhost:5432/your-db"
NEXTAUTH_SECRET="your-nextauth-secret"
NEXTAUTH_URL="http://localhost:3000"
GOOGLE_CLIENT_ID="your-google-client-id"
GOOGLE_CLIENT_SECRET="your-google-client-secret"


### 3. Setup the Database

```terminal
npx prisma migrate dev --name init
```

### 4. Run the development server 

```terminal
npm run dev
```

### Authentication Setup

Credential-based Sign In / Sign Up already implemented
Google Sign-In preconfigured
Easily extend by adding providers in /lib/auth.ts (NextAuth configuration)
Secure password storage via bcryptjs


### 🪄 UI Customization

Change your app name in the Sign-In and Sign-Up pages (/app/auth/sign-in and /app/auth/sign-up)
Modify branding text, logo, or background animation as per your app needs
Built with shadcn/ui for fast and consistent design updates

### 🧩 Extend the Starter Pack

You can easily:

Add new models in schema.prisma (e.g. Post, Todo, Project)
Integrate more OAuth providers
Create custom API routes using the App Router or Server Actions
Add middleware for route protection
Extend the UI library with more shadcn components


### 🧑‍💼 Project Structure

<img width="300" height="687" alt="Screenshot 2025-10-09 102903" src="https://github.com/user-attachments/assets/db7e30e6-b15f-4a10-ac77-bac42c98bdae" />


### 🧠 Tips

Always run npx prisma generate after modifying your schema
Update your .env file with valid credentials before running migrations
You can switch to any Prisma-supported database
Keep your NextAuth secret private and unique
Use server actions for clean data mutations in Next.js 14+

### ⚡ A perfect starter pack for developers who want to skip setup and start building full-stack Next.js apps instantly.

### 📜 License

This project is licensed under the MIT License – you’re free to use and modify it for personal or commercial projects.

🧡 Credits

Built with ❤️ by Sameer Saifi
Crafted with 💻 using Next.js, Prisma, and NextAuth.js

