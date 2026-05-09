# Skaha Heating & Air Ltd. — Website

Single-page static website for [skahaheating.com](https://skahaheating.com).

## Images

All images live in the `images/` folder. Current files:

| File | Used in | Notes |
|---|---|---|
| `images/logo-white.png` | Header | Horizontal logo with white text, used on navy background |
| `images/logo.png` | Footer | Horizontal logo with black/dark background, used on black footer |
| `images/van.jpg` | Hero section background | Photo of the Skaha Heating service van |
| `images/steve_photo.jpg` | About section | Headshot of Steve Martel, owner |

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
