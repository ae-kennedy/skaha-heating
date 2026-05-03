# Skaha Heating & Air Ltd. — Website

Single-page static website for [SkahahHeating.com](https://skahaheating.com).

## Add images

Create an `images/` folder in the repo root and add these three files:

| File | Use | Source |
|---|---|---|
| `images/logo.png` | Header (on white background) | Horizontal logo, white/transparent bg |
| `images/logo-white.png` | Footer (on dark background) | Horizontal logo with white text |
| `images/van.jpg` | Hero background + About section | Photo of Steve in the service van |

The site degrades gracefully without images — the hero shows a solid navy gradient fallback and logo areas remain blank.

## Deploy to GitHub Pages

1. Go to **Settings → Pages** in this repo
2. Set source to **Deploy from a branch → main → / (root)**
3. The site will be live at `https://ae-kennedy.github.io/skaha-heating/`

## Point skahaheating.com at GitHub Pages

1. Add a file named `CNAME` to the repo root containing exactly: `skahaheating.com`
2. In your domain registrar (likely GoDaddy), update DNS:
   - Add four `A` records pointing to GitHub Pages IPs:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - Add a `CNAME` record: `www` → `ae-kennedy.github.io`
3. DNS propagation takes up to 24 hours
