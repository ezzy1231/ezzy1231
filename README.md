# Edilu Densemo Tafesse

**Full-stack engineer building AI-powered web applications.**

I design and ship production systems where AI is genuinely part of the product — generative
features, speech pipelines, real-time streaming — on top of the infrastructure that keeps them
reliable under real traffic.

Based in Ethiopia · Open to freelance and contract work

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/edilu-densemo-tafesse-933571312/)
[![Email](https://img.shields.io/badge/Email-Ediludensemo1@gmail.com?style=for-the-badge&logo=gmail&logoColor=white)](mailto:Ediludensemo1@gmail.com)

---

## Featured work

Most of my product work lives in private repositories, so I've linked the running applications
and written up the engineering below. Happy to walk through the architecture on a call.

### HabeshaTTS — AI voice donations in Amharic

**Live:** <https://habeshatts.com/>

A donation platform for Ethiopian creators, with donations converted to natural Amharic speech
and streamed back to the donor in real time.

The interesting part is what sits behind the button:

- **Generative AI** — Gemini for content generation and conversational flows
- **Speech synthesis** — Google Cloud TTS with Amharic voice handling
- **Async work** — BullMQ job queues on Redis, so a long TTS render never blocks a request
- **Real-time delivery** — Socket.IO pushes rendered audio to the browser as it completes
- **Multiple front doors** — web app plus a Telegram bot, sharing one backend
- **Observability** — Raygun and Rollbar wired in from day one
- **Payments & auth** — Stripe, JWT sessions, OTP-based streamer onboarding, rate limiting

**Stack:** Node.js · Express · Socket.IO · BullMQ · Redis · PostgreSQL · Gemini · Google TTS · Docker

**▶ Watch the demo:** <!-- add your HabeshaTTS demo video link here --> _[link coming soon]_

---

### UrbanExplore — discovery and booking for Addis Ababa

**Live:** <https://urbanexplore.netlify.app/>

A Turborepo monorepo for a local marketplace covering restaurants, events, hotels and rides.

- **Monorepo architecture** — Turborepo + pnpm workspaces across web, API and shared packages
- **Geospatial data** — PostgreSQL with PostGIS, Prisma as the data layer
- **Auth and data security** — Supabase Auth with Row Level Security, so authorisation is enforced
  in the database rather than trusted from the client
- **Complex query surface** — PL/pgSQL RPCs and stored procedures for search and booking logic
- **Maps** — Google Maps JS, Places and Geocoding APIs for address autocomplete and routing
- **Real-time backend** — NestJS, Redis, Docker Compose for local infra

**Stack:** Next.js · NestJS · TypeScript · Prisma · PostGIS · Supabase · Redis · Docker · Turborepo

---

### EzhuFl

**Live:** <https://ezhu-fl.vercel.app/>

A TypeScript web application deployed on Vercel.

**Stack:** TypeScript · Next.js · Vercel

---

## How I work

- **AI that earns its place** — I reach for a model when it's the right tool, not because it's trending
- **Production-first** — queues, retries, rate limits, structured errors and monitoring are part of the build, not an afterthought
- **Security by default** — RLS in the database, secrets never committed, input validated at every boundary
- **Ship end to end** — schema design, API, frontend, deployment and observability

---

## Toolbox

| Area | Technologies |
|---|---|
| **Languages** | TypeScript, JavaScript (ESM), Node.js, SQL, Bash, PowerShell |
| **Frontend** | Next.js, React, Zustand, Tailwind CSS |
| **Backend** | Node.js, Express, NestJS, REST, WebSockets (Socket.IO) |
| **AI / ML** | Gemini (`@google/genai`), Google Cloud Text-to-Speech, prompt engineering, streaming inference |
| **Data** | PostgreSQL, PostGIS, Prisma, PL/pgSQL, Redis, BullMQ, SQLite |
| **Auth & Security** | Supabase Auth, Row Level Security, JWT, OAuth, Zod validation, rate limiting |
| **Payments & Messaging** | Stripe, Telegram Bot API |
| **Infrastructure** | Docker, Docker Compose, Nginx, Kubernetes, GitHub Actions, GitLab CI, Vercel |
| **Observability** | Raygun, Rollbar, Sentry-style error tracking |

---

## Get in touch

Found something interesting, or have a project in mind?

- **Email** — [Ediludensemo1@gmail.com](mailto:Ediludensemo1@gmail.com)
- **LinkedIn** — [edilu-densemo-tafesse](https://www.linkedin.com/in/edilu-densemo-tafesse-933571312/)

<!--
TODO for you:
  1. Confirm the email address (gmail.com vs whatever you intended)
  2. Add the HabeshaTTS demo video link under its section above
  3. Add a real portfolio site URL once you have one
-->