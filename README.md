# Annie Rose + Jjang Digitals by Rose: setup guide

## What you have
- `index.html`: the whole website (pages switch without reloading)
- `data/content.json`: ALL your content (products, portfolio, bio, links)
- `admin/`: the dashboard at `yoursite/admin` (Decap CMS, free)
- `images/`: uploaded photos land here

## Publish it (free)
1. Make a free GitHub account, create a new repository, and upload everything in this folder.
2. Make a free Cloudflare account > Workers and Pages > Create > Pages > Connect to Git > pick your repo. Leave build settings empty, output directory `/`. Deploy. You get a free `yourname.pages.dev` link with SSL.
3. Open `admin/config.yml` and replace `YOUR-GITHUB-USERNAME/YOUR-REPO-NAME` with your repo.
4. Admin login needs a small free "OAuth" helper so GitHub can let you sign in. Search "Decap CMS GitHub OAuth Cloudflare Workers" and follow a current tutorial, then put its address in `base_url` in `config.yml`. This is the one technical step. Ask me and I'll walk you through it.

## Update the site (no code)
Go to `yoursite/admin`, sign in, open "All content". You can add or edit products, prices, photos, stock (0 = sold out), variations (comma separated, e.g. `Small, Large`), portfolio projects, bio, services and contact links. Click Publish and the site updates in about a minute.
Backup option without the dashboard: edit `data/content.json` on GitHub directly.

## Gumroad (digital products)
Create the product on Gumroad, copy its link, and paste it in the product's "Gumroad product link". Gumroad handles payment and file delivery. Until a link is added, the button says "Purchase link coming soon".

## Physical products
Cart works in the browser. "Send order request" opens an email to you. Nothing is paid or confirmed until you reply with payment instructions (GCash, bank transfer) and confirm.

## Costs
Free: GitHub, Cloudflare Pages hosting and SSL, Decap CMS, the cart.
Gumroad: no monthly fee, but it takes a percentage per sale. Check gumroad.com/pricing for current rates.
Optional: a custom domain, roughly $10-15 a year.

## Before you launch, replace
Every item marked "Sample", the contact links, your photo, education and work details, and the testimonial.
