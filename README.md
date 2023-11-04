# E-Commerce Admin & Store

This is a repository for a Full Stack E-Commerce + Dashboard & CMS: Next.js 13 App Router, React, Tailwind, Prisma, MySQL.

## Demo

Ecommerce Admin: https://ecommerce-store-srikrishna7272.vercel.app/

Ecommerce Store: https://ecommerce-store-sk.vercel.app/

## Features

- Used Shadcn UI for the Admin!
- Admin dashboard is going to serve as both CMS, Admin and API!
- You will be able to control mulitple vendors / stores through this single CMS! (For example you can have a "Shoe store" and a "Laptop store" and a "Suit store", and our CMS will generate API routes for all of those individually!)
- You will be able to create, update and delete categories!
- You will be able to create, update and delete products!
- You will be able to upload multiple images for products, and change them whenever you want!
- You will be able to create, update and delete filters such as "Color" and "Size", and then - match them in the "Product" creation form.
- You will be able to create, update and delete "Billboards" which are these big texts on top of the page. You will be able to attach them to a single category, or use them standalone (Our Admin generates API for all of those cases!)
- You will be able to Search through all categories, products, sizes, colors, billboards with included pagination!
- You will be able to control which products are "featured" so they show on the homepage!
- You will be able to see your orders, sales, etc.
- You will be able to see graphs of your revenue etc.
- Authentication using clerk.
- Order creation
- Stripe checkout
- Stripe webhooks
- MySQL + Prisma + PlanetScale

## Run Locally

Clone the project

```bash
  git clone https://github.com/srikrishna7272/ecommerce-admin.git
```

Install dependencies

```bash
  npm install
```

Add Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=`

`CLERK_SECRET_KEY=`

`NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in`

`NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up`

`NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/`

`NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/`

`DATABASE_URL=''`

`NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=""`

`STRIPE_API_KEY=`

`FRONTEND_STORE_URL=http://localhost:3001`

`STRIPE_WEBHOOK_SECRET=`

Connect to PlanetScale and Push Prisma

```bash
  npx prisma generate

  npx prisma db push
```

Start the app

```bash
  npm run dev
```
