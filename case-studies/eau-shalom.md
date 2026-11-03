# Eau Shalom: a business operating system, run from two continents

**Client:** Eau Shalom, a bottled-water production and delivery business in Burkina Faso, with operations managed remotely from the US East Coast.

**Problem:** Orders, deliveries, and cash collection ran on memory and phone calls, across a 4-hour time difference, with no shared source of truth between the owner, the site manager, the drivers, and the vendors.

**What I built:** A Flutter app for the owner and the site manager, backed by Supabase, plus a WhatsApp worker so boutiques can order and check their balance where they already talk. 13+ tables with row-level security enforce every role's data access at the database layer. 22 schema migrations and 63 automated tests cover the work.

**Timeline:** Core build May-June 2026, hardened through September 2026 for rollout.

**My role:** Sole engineer. Domain modeling, schema and security design, the full Flutter client, the WhatsApp worker, tests, and deployment.

**Stack:** Flutter/Dart, Supabase (PostgreSQL, RLS, Auth), Cloudflare.

**What it demonstrates:** Multi-tenant thinking (role isolation enforced in the database, not just the UI), disciplined testing on a real business workflow, and building for non-technical users in a low-bandwidth environment, across languages and continents.
