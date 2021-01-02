# Next.js boilerplate for creating fast, cms-baked (eCommerce) websites
This project is the base I use when creating websites. It is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app) and using [GraphCMS](https://graphcms.com/) as it underlying headless CMS and Stripe payments for the eCommerce part. It can be adapted to use another CMS, like strapi, contentful, or any other headless CMS providing a multi-language graphql API.

## Focus
This website tries to focus on best practices in the field of website creation. It focuses on:
- Providing good natural SEO optimization
  - Using `next/head`
  - Providing unique, per-page meta tags directly from the CMS
  - Auto generating branded social-media images using `puppeteer` on a serverless function
  - Providing all the required favicon images
  - Providing the required `robots.txt` and `manifest.webmanifest` files
- Using the appropriated HTML delivery mechanism
  - Using static site generation where possible
  - Using server side rendering for dynamic routes
  - Using client side code for live dynamic content
- Using custom Stripe payments for the ecommerce
- Using i18n with `next-translate`, next.js localized routing, localized content straight from the CMS and native number formatting using `Intl.NumberFormat`
- Using `React.Context` for global state (e.g. loading or cart state)
- Using Tailwinf in combination of CSS modules for an optimized performance and a minimal effort
- Providing the best setup for a frictionless deployment with `vercel`

## Running the website locally
First, rename the `sample.env` file to `.env` and adapt the values.

Then, run the development server:

```bash
npm run dev
# or
yarn dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `pages/index.js`. The page auto-updates as you edit the file.

[API routes](https://nextjs.org/docs/api-routes/introduction) can be accessed on [http://localhost:3000/api/hello](http://localhost:3000/api/hello). This endpoint can be edited in `pages/api/hello.js`.

The `pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
