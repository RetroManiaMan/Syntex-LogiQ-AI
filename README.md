# LogiQ AI

[![Website](https://img.shields.io/badge/demo-online-brightgreen)](https://logiq-ai.base44.app/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![CI](https://github.com/YOUR_ORG/LOGIQ_AI/actions/workflows/ci.yml/badge.svg)](https://github.com/YOUR_ORG/LOGIQ_AI/actions)

> LogiQ AI — your smart assistant for X, Y, Z. Built with speed, privacy, and delightful UX in mind.
## LogiQ AI ScreenShots!
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 11 46 PM" src="https://github.com/user-attachments/assets/9c04de6d-d1d2-48f6-bc7a-d35d4344f540" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 12 35 PM" src="https://github.com/user-attachments/assets/e181240a-017f-4773-b06e-cf5f8b35547b" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 12 49 PM" src="https://github.com/user-attachments/assets/65dc4d42-d151-4c6f-aedc-ee85d90f0a77" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 15 06 PM" src="https://github.com/user-attachments/assets/a6a7a639-0702-4593-930b-5773f1828380" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 15 14 PM" src="https://github.com/user-attachments/assets/2db54fb3-f8e5-4645-8b70-b91dd82854df" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 15 21 PM" src="https://github.com/user-attachments/assets/69e36b7d-4473-443c-872c-5cadbf4ed5e3" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 15 28 PM" src="https://github.com/user-attachments/assets/9dd1e4f0-723e-4a46-8a7b-5dc7fe657d93" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 15 39 PM" src="https://github.com/user-attachments/assets/f0746e6b-bea1-4682-baea-f34a7f4fb63f" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 15 56 PM" src="https://github.com/user-attachments/assets/b3a5498e-d7b7-4175-9575-adf27ab507f1" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 16 03 PM" src="https://github.com/user-attachments/assets/ef952e0b-0ae8-4f4b-9002-059c8d09be31" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 16 12 PM" src="https://github.com/user-attachments/assets/6a7575e1-bca8-450b-8d51-cd17bee0eee8" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 16 21 PM" src="https://github.com/user-attachments/assets/d76e7035-89bd-4b07-a112-6e8e886f56b2" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 16 33 PM" src="https://github.com/user-attachments/assets/6e074f47-d65b-4de9-81e8-188281fd318b" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 22 36 PM" src="https://github.com/user-attachments/assets/f70cb0dd-81e6-489f-b4aa-caed06a43b7f" />
<img width="1470" height="799" alt="Screenshot 2025-10-09 at 10 22 51 PM" src="https://github.com/user-attachments/assets/48466d6f-1d5a-4159-93b4-b8e18104812b" />
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
