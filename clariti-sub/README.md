# Clariti — Subscription Edition (clariti.global)

Static site restructuring Clariti around three monthly subscription plans (BOXAS model):
Advisory On-Tap ($2,950/mo, live offer) · Program Assurance ($5,950/mo) ·
Transformation Office ($9,950/mo, flagship).

## Structure
- index.html — home (decision positioning + rate board)
- plans/{advisory-on-tap|program-assurance|transformation-office}/index.html
- about/ · contact/ · 404.html · sitemap.xml · robots.txt · .htaccess (Apache)
- assets/css/main.css (Clariti tokens: Navy #0E1858, Signal Orange #EC4E20, Playfair Display + DM Sans)
- assets/js/main.js (mobile nav)

## Deploy
Upload the folder contents to the web root (same host pattern as the previous clariti-site build).
Point dxadvisory.com → 301 redirect to clariti.global, keeping /score working.

## To do before launch
1. Drop images into assets/images/home/ (leading.png, buildings.png) — panels degrade gracefully without them.
2. Wire forms to your form handler (currently action="#").
3. Confirm prices; all shown ex GST.
