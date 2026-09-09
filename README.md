# Services by Dela v2

Ghana-first managed professional services marketplace.

## What is included
- Mobile-first UI with fixed-header spacing corrected
- Secure admin login using an HttpOnly session cookie (password is never placed in the URL)
- Rate-limited admin login attempts
- Security headers
- Persistent PostgreSQL storage when DATABASE_URL is set
- Safe local JSON fallback for development only
- Five initial professionals seeded in the database
- Job lifecycle: NEW → ACCEPTED → CUSTOMER CONTACTED → JOB SCHEDULED → COMPLETED → CUSTOMER CONFIRMED → FEE DUE → PAID / DISPUTED
- Admin matching suggestions by service and area
- WhatsApp click-to-contact links for support, customer follow-up, and professional follow-up without publicly exposing professional numbers
- Support tickets and professional applications
- Health check at /api/health

## Render setup
1. Keep the existing web service on the Free plan for testing.
2. Create a Render Postgres database in the same region as the web service.
3. Add its internal database URL to the web service as DATABASE_URL.
4. Keep ADMIN_PASSWORD secret.
5. Deploy the main branch.

Important: Render's Free Postgres is for testing and expires after 30 days. Upgrade the database to a paid plan before relying on it for real customer records.

## Public contact
0541721528
