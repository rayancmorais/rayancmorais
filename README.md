# Hey there, I'm Rayan 👋

Full-stack developer from Juiz de Fora, Brazil. I came into software from an unusual direction — I worked in healthcare before this, and the habits stuck: rigid protocols, zero tolerance for error, and a reflex for edge cases nobody thought to check. That's the lens I bring to code.

I build things that run in production, not just in localhost. Right now I'm working on **Vasc-Review**, a continuing medical education platform used by vascular surgeons (published on the App Store and Play Store), while shipping my own projects on the side.

## 🛠️ What I work with

**Front-End:** React, Next.js, React Native, TypeScript, Tailwind CSS, Styled Components

**Back-End:** Node.js, NestJS, Fastify, Express, Go

**Data & Infra:** PostgreSQL, MongoDB, Redis, BullMQ, RabbitMQ, Meilisearch, Docker, AWS Lambda, Railway

**Practices:** DDD, Clean Architecture, TDD (Vitest/Jest), event-driven architecture, CI/CD with GitHub Actions

## 🚀 Things I've built

**[CupomManiac](https://cupommaniac.com.br)** — *live in production*  
Affiliate coupon platform for the Brazilian market, built from scratch to its own domain. Syncs thousands of coupons from 5 affiliate networks (Lomadee, Admitad, Awin, Amazon, Mercado Livre) through a common adapter interface, with real-time search via Meilisearch and async processing via BullMQ. Notable work: refactored an N+1 that was locking the database under load into batched upserts, and solved cross-origin cookie blocking between Railway and Vercel with server-side proxy routes.  
`Next.js 15` `TypeScript` `Fastify` `Prisma` `PostgreSQL` `Redis` `BullMQ`

**[Crash Game](https://github.com/rayancmorais/fullstack-challengeRayancm)** — *technical challenge*  
Real-time multiplayer crash game where services communicate exclusively over RabbitMQ — no direct HTTP between them, so the Wallet stays the single source of truth for balances. Domain layer is pure TypeScript (zero framework), covered by 91 unit tests and 11 E2E scenarios. Money handled as BigInt cents to eliminate floating-point drift, and crash points are provably fair via HMAC-SHA256.  
`NestJS` `Bun` `DDD` `RabbitMQ` `Kong` `Keycloak` `WebSocket` `Docker`

**Lux Lab** — [live site (BR)](https://luxlabbr.vercel.app) · [code (EU version)](https://github.com/rayancmorais/luxeLab)  
Multi-market e-commerce platform for Brazil and the EU. A single `Supplier` interface implemented by BR and EU providers routes orders by delivery country, so adding a supplier or a market never touches the order flow. Region-aware pricing computes local currency, margin, and destination-country tax in isolated stages, and an AI shopping assistant streams over SSE within Lambda's 29-second connection ceiling. The live site is the Brazilian version; the public code is the European one it was adapted from.  
`Go` `Gin` `MongoDB` `Next.js 15` `AWS Lambda` `MercadoPago` `Stripe` `OAuth2/OIDC`

## 🔭 Currently building

**NexusAI** — a distributed e-commerce platform with semantic search and real-time AI chat, built across Go, Node.js/Bun, Python and Next.js, with gRPC contracts managed by Buf and an OpenAPI-first workflow. I'm documenting the build publicly, phase by phase.

## 📬 Let's talk

I'm open to full-stack opportunities — remote friendly, and I work in English (C1).

**Portfolio** — [rayancmorais.com.br](https://rayancmorais.com.br)  
**LinkedIn** — [linkedin.com/in/rayancmorais](https://linkedin.com/in/rayancmorais)  
**Email** — [rayan_cm2021@icloud.com](mailto:rayan_cm2021@icloud.com)

