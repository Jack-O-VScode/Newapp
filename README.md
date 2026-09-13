# APEX MART

Promo site for APEX MART — Steam wallet codes and WMMT6 PC setup.
Single static HTML page, no build step, no dependencies.

## Add your images

Put these in `assets/` (see `assets/README.md`):
`logo.png`, `review-1.png`, `review-2.png`, `review-3.png`

## Editing

Everything is in `index.html`. The bits you'll most likely want to change:

- **Review badges** — search for `EDIT ME` to correct the badge labels.
- **Rating / review count** — search for `4.75` and `64`.
- **Contact** — Instagram handle appears in 3 places; email is assembled in
  the script at the bottom to slow down scrapers.
- **Products** — the two `<article class="prod">` blocks.
- **Orders** — `FORM_KEY` at the top of the script. A free Web3Forms access
  key (web3forms.com). Empty = the Send button falls back to opening the
  visitor's email app instead of posting the order.
- **Booking** — `BOOK_URL` and `PRICE` at the top of the script. BOOK_URL is
  the Cal.com page (it handles slot choice and payment together). Set PRICE
  only once Stripe is connected on that Cal event; until then the button
  says "Book a session" rather than promising a payment step.

## Publishing to GitHub Pages

1. Push to GitHub.
2. Repo → **Settings → Pages** → Source: `Deploy from a branch` → pick the
   branch, folder `/ (root)` → Save.
3. Live in a minute or two.

## Custom domain

1. Buy the domain (Cloudflare Registrar sells at cost).
2. Settings → Pages → **Custom domain** → enter it → Save. This writes a
   `CNAME` file into the repo.
3. At your registrar, add for the root domain four A records:
   `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   and a CNAME for `www` → `<username>.github.io`
4. Once DNS resolves, tick **Enforce HTTPS**.
