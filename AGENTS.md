# AGENTS.md

## Project context

This is a Django MVP for an anonymous/report-based platform.

## Current decisions

- Backend: Django
- Database: PostgreSQL
- Cache/rate limiting: Redis
- Hosting target: Oracle Cloud Free Tier VM
- CDN/WAF: Cloudflare
- Media later: Cloudflare R2
- MVP is text-only
- No pre-approval moderation
- Use report-based moderation
- Use Django Admin as MVP moderation queue

## Rules

- Do not add media/audio unless explicitly asked.
- Do not build a custom moderation dashboard yet.
- Prefer small, high-confidence changes.
- Before changing code, inspect the existing structure.
- After changing code, run Django checks/tests where possible.
- Explain changed files and why.
- Ask before adding new production dependencies.
- Never touch secrets or environment files.
- Keep legal/compliance-related behavior conservative.
