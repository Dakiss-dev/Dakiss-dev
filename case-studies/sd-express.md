# SD Express: from rented AI platform to owned infrastructure in 3 days

**Client:** SD Express, a live package-shipping business in Ouagadougou, Burkina Faso.

**Problem:** The business ran on a GenSpark-generated website it did not own or control. No code access, no data ownership, no way to extend it, and the platform bill kept running.

**What I built:** A full migration to owned infrastructure on Cloudflare: Pages for the site, Pages Functions for the backend, D1 (SQLite) for the database. Admin pages protected by password login with HMAC session cookies enforced by server-side middleware. GitHub Actions auto-deploys on every push to main, so the client's site updates with zero manual steps.

**Timeline:** Migration completed in about 3 days (May 23-25, 2026). Live at [sd-express.pages.dev](https://sd-express.pages.dev).

**My role:** Sole engineer. Data migration, backend, authentication, deploy pipeline, and handoff to the owner.

**Stack:** Cloudflare Pages, Pages Functions, D1, GitHub Actions.

**What it demonstrates:** Shipping a production system solo and fast for a real operating business, in French, with the client 8,000 km away. The handoff left the owner with infrastructure he owns outright: repo, database, and deploys, at near-zero monthly cost.
