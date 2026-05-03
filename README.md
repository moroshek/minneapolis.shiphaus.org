# minneapolis.shiphaus.org

Static event presentations for the Shiphaus Minneapolis chapter.

## Routes

- `/msp1` — MSP Shiphaus #1 (May 3, 2026)
- `/` — redirects to the latest event

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000/msp1.html
```

## Deploy

Hosted on Netlify. Push to `main` triggers auto-deploy.

```bash
# manual deploy via CLI:
netlify deploy --prod
```

In the Netlify dashboard: **Domain settings** → add custom domain `minneapolis.shiphaus.org` → follow the DNS prompt (CNAME `minneapolis` → `<site>.netlify.app`, or use Netlify DNS for the apex if shiphaus.org is delegated).

## Convention

Modeled on `chicago.shiphaus.org/chi2`. Each event is a single self-contained HTML file at `/<eventslug>` (e.g. `/msp1`, `/msp2`).
