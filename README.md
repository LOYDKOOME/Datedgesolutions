# Datedge Solutions

Static website for Datedge Solutions: data analytics, research, automation, IT support,
hospitality technology training and POS installations (Nairobi, Kenya).

## Structure
```
wrangler.jsonc        Cloudflare Workers static-assets config
public/
  index.html          Main page
  styles.css          Shared styles
  app.js              Project cards, mobile menu, footer year
  dashboards.html     Interactive sample dashboards page
  dashboards.css      Dashboard page styles
  dashboards.js       Dashboard data, charts, tabs, period selector
  chart.js            Chart.js v4.6.1 (MIT) bundled locally
```

## Run locally
```
cd public
python3 -m http.server 8000
```
Then open http://localhost:8000

## Deploy to Cloudflare
Connect this repo in Cloudflare (Workers & Pages). Build command: none.
Deploy command: `npx wrangler deploy`. The `wrangler.jsonc` points to `./public`.
