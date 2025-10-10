# LogiQ AI

[![Website](https://img.shields.io/badge/demo-online-brightgreen)](https://logiq-ai.base44.app/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![CI](https://github.com/YOUR_ORG/LOGIQ_AI/actions/workflows/ci.yml/badge.svg)](https://github.com/YOUR_ORG/LOGIQ_AI/actions)

> LogiQ AI — your smart assistant for X, Y, Z. Built with speed, privacy, and delightful UX in mind.
![LogiQ AI Screenshots]
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 11 46 PM" src="https://github.com/user-attachments/assets/58c7a522-c1bf-441a-96ae-0e783c9f1bbe" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 12 35 PM" src="https://github.com/user-attachments/assets/b394b19f-85f8-4e7b-9fba-4d52b0ea9c55" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 12 38 PM" src="https://github.com/user-attachments/assets/d31bd925-05a2-4687-97f4-6841abdcac65" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 12 42 PM" src="https://github.com/user-attachments/assets/b5a424d5-c6ba-4a98-96df-32852fb44681" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 12 49 PM" src="https://github.com/user-attachments/assets/e1c01d22-49c0-45a1-a747-dcbad56359ff" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 15 06 PM" src="https://github.com/user-attachments/assets/e84be833-d679-45e5-b6d2-70d9cea16a8d" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 15 14 PM" src="https://github.com/user-attachments/assets/a61cb4a5-a0d9-439a-a2c6-558a77d393a7" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 15 21 PM" src="https://github.com/user-attachments/assets/5de1cd80-9b22-403b-8d14-d881830de957" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 15 28 PM" src="https://github.com/user-attachments/assets/59f4347a-82a5-47bb-a417-b3e26df11b97" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 15 39 PM" src="https://github.com/user-attachments/assets/6e0ae628-8c6a-4d06-be7c-46a7f7f3338f" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 15 56 PM" src="https://github.com/user-attachments/assets/4497b633-4121-4f78-9258-2ebb4e69c6c2" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 16 03 PM" src="https://github.com/user-attachments/assets/91918967-a84b-488e-abe4-ab4a9c68e581" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 16 12 PM" src="https://github.com/user-attachments/assets/eac7e8a8-c9de-400a-8e9f-e33ebbf2cd4e" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 16 21 PM" src="https://github.com/user-attachments/assets/7f17b17e-c5b9-4d36-8c82-5f55c03e0fc8" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 16 33 PM" src="https://github.com/user-attachments/assets/29d5dbf2-dee2-4094-bae7-dcc4ed895998" />
<p align="center">
  <img src="assets/homepage.png" alt="LogiQ AI Screenshot" width="800"/>
</p>

## Demo
https://logiq-ai.base44.app/ — live production instance.

## Overview
Short pitch: server-backed frontend + LLM integrations, conversational worker queue, auth, and analytics.

### Key features
- Real-time chat UI
- Role-based access
- Extensible plugins (connectors for APIs)
- Audit logs and analytics
- CI/CD and containerized deployment

### Tech stack
- Frontend: Next.js / React (adjust if you used something else)
- Backend: Node.js / Express / FastAPI (replace accordingly)
- Datastore: PostgreSQL (or your DB)
- Auth: Auth0 / NextAuth / Custom JWT
- Hosting: Base44 / Vercel / Netlify / Docker

## Architecture
See `docs/architecture.md` for a high level diagram and decisions.

## Quickstart (local)
> Assumes Node.js (v18+), Docker optional.

1. Clone
```bash
git clone https://github.com/YOUR_ORG/LOGIQ_AI.git
cd LOGIQ_AI
```

2. Copy env template
```bash
cp .env.example .env
# Fill in the vars (OPENAI_KEY, DATABASE_URL, NEXT_PUBLIC_BASE_URL, etc.)
```

3. Install & run
```bash
npm install
npm run dev
# or: docker compose up --build
```

4. Open http://localhost:3000

## Environment variables
See `.env.example`. Never commit real secrets.

## Deploying
### Vercel (recommended for Next.js)
- Connect repo to Vercel
- Set VERCEL_TOKEN and other env vars in Vercel dashboard
- Push to `main` to trigger deploy

### Docker
```bash
docker build -t logiq-ai .
docker run --env-file .env -p 3000:3000 logiq-ai
```

## Contributing
Please read `CONTRIBUTING.md` and `CODE_OF_CONDUCT.md`. We're happy to accept PRs and issues.

## Security
See `SECURITY.md` for reporting vulnerabilities.

## License
MIT — see `LICENSE`.

## Maintainers
- Your Name – @yourgithub

## Acknowledgements
Thanks to Base44 for hosting.
