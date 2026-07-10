# Eau Shalom: a 4-role business operating system, run across two continents

**Client:** Eau Shalom, a bottled-water production and delivery business in Burkina Faso, with operations managed remotely from the US East Coast.

**Problem:** Orders, deliveries, and cash collection ran on memory and phone calls, across a 4-hour time difference, with no shared source of truth between the owner, the site manager, the drivers, and the vendors.

**What I built:** A Flutter app with four distinct roles (owner, manager, driver, vendor), each seeing exactly their slice of the operation, backed by Supabase: 13+ tables with row-level security so every role's data access is enforced at the database layer, 20 schema migrations, and a WhatsApp worker for notifications where WhatsApp is the default communication channel. The end-to-end loop (order placed → delivery assigned → delivered → cash collected) is covered by 57 passing automated tests.

**Timeline:** Core build May-June 2026, shipped and in live use.

**My role:** Sole engineer. Domain modeling, schema and security design, the full Flutter client, the WhatsApp worker, tests, and deployment.

**Stack:** Flutter/Dart, Supabase (PostgreSQL, RLS, Auth), Cloudflare.

**What it demonstrates:** Multi-tenant thinking (role isolation enforced in the database, not just the UI), disciplined testing on a real business workflow, and shipping software that non-technical users in a low-bandwidth environment actually operate every day, across languages and continents.
