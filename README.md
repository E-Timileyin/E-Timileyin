# Eyiowuawi Timileyin

**Backend-leaning fullstack engineer. Go, TypeScript, APIs and platform infrastructure. Lagos, Nigeria.**

Contract engineer at [Knurb Ltd](https://knurbdesign.com), a brand and design studio. I'm also building [SkillIsle](https://skillisle.com), a gamified learning platform. a direct-booking platform for [Favoured Properties Ltd](https://favoured-homes.vercel.app), and contributing to the [BTE platform](https://github.com/btetotheworld).

I work in Go and TypeScript, with PostgreSQL, Redis and Docker underneath. I care about clear service boundaries, authorization enforced at the data layer, and systems that are boring to operate. Open to remote roles.

## Selected work

**[SkillIsle](https://skillisle.com)** · Full-stack developer · Go (Chi), PostgreSQL, Next.js, Phaser,Asynq, Prometheus etc

A gamified learning platform for learners with special educational needs and disabilities (SEND): multiplayer games, parent and educator dashboards, analytics, Stripe billing and Google OAuth/OTP sign-in, deployed with Docker, CI/CD, Vercel and a VPS. **Why it matters:** parents and educators can see how a learner is actually doing, and scoring runs on the server, so the results can be trusted.

**[Favoured Homes](https://favoured-homes.vercel.app)** · Client project · Node.js, TypeScript, Hono, Drizzle, PostgreSQL, Redis, Next.js

A direct-booking platform for Favoured Properties Ltd, a short-stay rental operator in Manchester and Bolton: guest site, booking flow and an admin dashboard on a Hono API. **Why it matters:** guests book direct instead of through marketplaces, so the operator avoids their fees. The channel manager sits behind a port/adapter layer, so Smoobu can be swapped for Beds24 without touching booking logic.

**[Favoured Homes](https://www.mbitaownu.com/)** · Freelance, fullstack · React 19, Vite, Hono, Payload CMS, PostgreSQL, Docker, ci/cd, nginx, worker

A portfolio and professional-record site for a client, built as one TypeScript app: a React SPA and Hono API in a single Docker image, Payload CMS on Neon Postgres and a custom admin console. **Why it matters:** a portfolio is normally static, but this client needed to edit every word themselves, including their career record and publications, without a developer. Public forms are Zod-validated, reader replies are moderated, unpublished posts are excluded in the query so they can't leak, and deploys go through an approval-gated pipeline that health-checks the service.

**[Knurb](https://knurbdesign.com)** · Contract, fullstack · Next.js 16, React 19, GSAP, Lenis, Tailwind CSS, etc

A website and content admin for Knurb, a brand design studio: GSAP-driven motion and case-study pages, plus an admin panel to add, edit and delete projects, project details and site content. **Why it matters:** the studio sells visual craft, so its own site has to prove it, and originally every new case study meant a code change and a deploy. Now the team publishes on its own.

**[Sail](https://github.com/E-Timileyin/Sail-CLI)** · Personal project · Go, Cobra, Viper, Docker, SSH

A CLI that deploys Dockerized apps to remote servers over SSH, with rollbacks and per-environment config (dev, staging, production). **Why it matters:** it turns a manual, error-prone server deploy into one repeatable command, with a way back when a release goes wrong.

**[BTE Platform](https://github.com/btetotheworld/bte-campus-app)** · Contributor · Next.js, Supabase (PostgreSQL)

The operations platform for Believers Tech Expo: people, campus chapters and role-based access enforced with row-level security. Still in development. **Why it matters:** chapters are run by student leads who graduate, so the platform keeps the records and access rules that let a chapter outlast them. I have two merged PRs: `people.kind`, which separates team from community members (community members aren't publicly listed by default), and a `join_applications` table for the volunteer apply flow, where applicants can only write their own application. Each ships its RLS policies and tests in the same migration.

## How I approach systems

- **Untrusted clients.** In SkillIsle, scoring is server-authoritative behind a WebSocket hub. The client renders; the server decides.
- **Vendor boundaries behind interfaces.** In Favoured Homes, the channel manager is an adapter, so replacing a vendor is a new adapter, not a rewrite.
- **Authorization in the query, not after the fetch.** On Mbitaownu.com, unpublished posts are excluded by a query constraint, so a draft can't leak through any endpoint.
- **Deploys that verify themselves.** The Mbitaownu.com pipeline polls a health endpoint after every deploy and fails the workflow if the service isn't actually serving.

## Where I'm heading

Moving from building features to designing systems: fault-tolerant services, clear service boundaries and data flow, and honest trade-offs between scalability, reliability and complexity. The aim is system design and platform engineering, built on shipping real systems first.

## Stack

- **Languages:** Go, TypeScript, JavaScript
- **Backend:** Gin, Chi, Hono, Node.js (Express), REST, WebSockets, JWT, OAuth2, Payload CMS
- **Data:** PostgreSQL, Redis, Drizzle, Prisma, Redis
- **Infra:** AWS,Docker, GitHub Actions, CI/CD, Render, Vercel, VPS deployment
- **Frontend:** React, Next.js, Tailwind CSS, GSAP

## Contact

- Portfolio: [eyiowuawitimileyin.com](https://eyiowuawitimileyin.com)
- Email: [hello@eyiowuawitimileyin@gmail.com](mailto:hello@eyiowuawitimileyin@gmail.com)
- x: [https://x.com/Eyiow_Tim](https://x.com/@Eyiow_Tim).
