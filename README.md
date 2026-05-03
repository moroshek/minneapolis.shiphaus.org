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

```bash
vercel --prod
```

Then in the Vercel dashboard, add the custom domain `minneapolis.shiphaus.org` and follow the DNS instructions (usually a CNAME on the `minneapolis` subdomain to `cname.vercel-dns.com`).

## Convention

Modeled on `chicago.shiphaus.org/chi2`. Each event is a single self-contained HTML file at `/<eventslug>` (e.g. `/msp1`, `/msp2`).
