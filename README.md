# SolidJS Web App

Frontend utama berbasis SolidStart (SSR) untuk website portfolio.

## Stack

- SolidStart + SolidJS
- Tailwind CSS
- Auth.js (Discord OAuth)
- API client ke Rust API dan Elysia API

## Run Locally

```bash
bun install
bun run dev
```

Default local URL: `http://localhost:4090`

## Scripts

```bash
bun run dev
bun run build
bun run start
bun run lint
bun run check
```

## Environment Variables

Required (server):

```env
DISCORD_ID=
DISCORD_SECRET=
AUTH_SECRET=
```

Optional:

```env
AUTH_TRUST_HOST=true
AUTH_URL=http://localhost:4090/api/auth
GOOGLE_CLIENT_ID=
VITE_GOOGLE_CLIENT_ID=
VITE_RUST_API=http://localhost:4091
VITE_ELYSIA_API=http://localhost:4092
```

Jika `VITE_RUST_API` / `VITE_ELYSIA_API` tidak diisi, app memakai fallback:

- localhost saat development
- domain production saat deployment
