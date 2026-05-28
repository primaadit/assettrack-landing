# AssetTrack Landing Page

Static landing page for AssetTrack — SaaS Asset Management System by Prima Praditya.

**Single file:** `index.html` — no build step, no dependencies, open directly in any browser.

---

## Deploy Instructions

### Vercel (Recommended — fastest)

1. Push folder to a GitHub repository
2. Go to [vercel.com](https://vercel.com) → New Project → Import repo
3. Framework preset: **Other** (leave all settings default)
4. Click **Deploy**
5. Done — live in ~30 seconds with HTTPS

**Or via Vercel CLI:**
```bash
npm i -g vercel
cd assettrack-landing
vercel --prod
```

---

### Netlify

**Option A — Drag & Drop (instant):**
1. Go to [app.netlify.com](https://app.netlify.com)
2. Drag the `assettrack-landing` folder onto the deploy area
3. Done — live in seconds

**Option B — Git-connected:**
1. Push to GitHub
2. Netlify → New site from Git → select repo
3. Build command: *(leave empty)*
4. Publish directory: `.` or `assettrack-landing`
5. Deploy

**Option C — Netlify CLI:**
```bash
npm i -g netlify-cli
netlify deploy --dir . --prod
```

---

### GitHub Pages

1. Push to a GitHub repo (e.g. `assettrack-landing`)
2. Go to repo **Settings → Pages**
3. Source: **Deploy from a branch**
4. Branch: `main`, folder: `/ (root)`
5. Save — live at `https://<username>.github.io/assettrack-landing/`

**For custom domain on GitHub Pages:**
- Add a `CNAME` file in the folder with your domain (e.g. `assettrack.id`)
- Configure DNS A record pointing to GitHub Pages IPs

---

### Self-Hosted (Nginx / Apache)

Copy `index.html` to your web root:

```bash
# Nginx
cp index.html /var/www/html/

# Apache
cp index.html /var/www/html/
```

No server-side processing needed — pure static file.

---

## Custom Domain

All three platforms support custom domains with automatic HTTPS (Let's Encrypt):

| Platform | Custom Domain | HTTPS |
|---|---|---|
| Vercel | Settings → Domains | Auto |
| Netlify | Site settings → Domain management | Auto |
| GitHub Pages | Settings → Pages → Custom domain | Auto |

---

## File Structure

```
assettrack-landing/
├── index.html    ← Single self-contained file (CSS + JS inline)
└── README.md     ← This file
```

---

## Contact

Built by **Prima Praditya**  
WhatsApp: [+62 812-2959-0817](https://wa.me/6281229590817)  
Email: primapraditya13@yahoo.co.id
