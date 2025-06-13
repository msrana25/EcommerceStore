# This repository is for a Full Stack E-Commerce Store website built using Next.js 13 App Router, React, Tailwind, Prisma, MySQL
For DEMO, use [Stripe Testing Cards](https://stripe.com/docs/testing)

# Key Features:

- Utilizes Shadcn UI for the Admin!
- The admin dashboard serves as both a CMS, Admin, and API.
- Manages multiple vendors/stores through this single CMS. For example, we can have a "Shoe store," a "Laptop store," and a "Suit store," and the CMS will generate API routes for each individually.
- Allows to create, update, and delete categories.
- Enables to create, update, and delete products.
- Supports uploading multiple images for products with the flexibility to change them whenever needed.
- Create, update, and delete filters such as "Color" and "Size" and match them in the "Product" creation form.
- Create, update, and delete "Billboards," which are prominent texts displayed on top of the page. These can be attached to a single category or used standalone. The Admin generates API routes for all of these cases.
- Offers a comprehensive search functionality across all categories, products, sizes, colors, and billboards with included pagination.
- Allows to control which products are marked as "featured," ensuring they appear on the homepage.
- Provides insights into your orders, sales, and more.
- Includes graphs to visualize your revenue.
- Incorporates Clerk Authentication.
- Supports order creation.
- Implements Stripe checkout and Stripe webhooks.
- Utilizes MySQL, Prisma, and PlanetScale for data management.

### Install packages

```shell
npm i
```

### Setup .env file


```js
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# This was inserted by `prisma init`:
# Environment variables declared in this file are automatically made available to Prisma.
# See the documentation for more detail: https://pris.ly/d/prisma-schema#accessing-environment-variables-from-the-schema

# Prisma supports the native connection string format for PostgreSQL, MySQL, SQLite, SQL Server, MongoDB and CockroachDB.
# See the documentation for all the connection string options: https://pris.ly/d/connection-strings

DATABASE_URL=''
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=""
STRIPE_API_KEY=
FRONTEND_STORE_URL=http://localhost:3001
STRIPE_WEBHOOK_SECRET=
```

### Connect to PlanetScale and Push Prisma
```shell
npx prisma generate
npx prisma db push
```


### Start the app

```shell
npm run dev
```

## Available commands

Running commands with npm `npm run [command]`

| command         | description                              |
| :-------------- | :--------------------------------------- |
| `dev`           | Starts a development instance of the app |
