# portfolio

This project is a starter [Next.js](https://nextjs.org) application generated with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app), configured for the App Router, JavaScript, and Tailwind CSS.

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.js`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Tech Stack

- Next.js App Router
- Tailwind CSS (via `@tailwindcss/postcss`)
- JavaScript modules with `jsconfig.json` path aliases
- Dockerized runtime via multi-stage `Dockerfile`
- Automated Docker builds via GitHub Actions

## Docker

Build the production image and run a container:

```bash
docker build -t portfolio .
docker run -p 3000:3000 portfolio
```

## CI/CD

A GitHub Actions workflow (`.github/workflows/docker-publish.yml`) builds the Docker image, pushes `tawadeshubham16/portfolio:latest`. Add the following repository secrets before triggering the workflow:

- `DOCKERHUB_USERNAME`
- `DOCKERHUB_TOKEN`

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
