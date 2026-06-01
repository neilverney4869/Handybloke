# The Helpful Bloke – Website

Static website for **Neil Verney – The Helpful Bloke**, a Canberra-based handyman and technology specialist.

**Live site:** https://handybloke.vercel.app  
**Custom domain (target):** https://thehelpfulbloke.com

---

## File Structure

```
/
├── index.html              # Home page
├── about.html              # About Neil page (with bio photo)
├── portfolio.html          # Completed jobs gallery
├── scheduler.html          # Book a time / scheduling
├── invoice.html            # Quote & Invoice (placeholder)
├── services-handyman.html  # Handyman services detail
├── services-property.html  # Property maintenance detail
├── services-tech.html      # Tech support detail
├── style.css               # Shared stylesheet
├── logo.png                # Brand logo
├── bio.jpeg                # Neil's photo (About page)
├── pallet-fence-stain-done.jpeg
├── frame-stain-done.jpeg
├── benchswing-set-done.jpeg
├── accessibility-ramp-done.jpeg
├── robots.txt
├── sitemap.xml
└── vercel.json             # Vercel deployment config
```

---

## How to Deploy

### Step 1 – Push to GitHub

1. Go to https://github.com/neilverney4869/Handybloke
2. If the repo is empty, initialise it:

```bash
git init
git remote add origin https://github.com/neilverney4869/Handybloke.git
git add .
git commit -m "Initial deploy – The Helpful Bloke website"
git branch -M main
git push -u origin main
```

If the repo already has content, pull first:

```bash
git pull origin main --allow-unrelated-histories
# resolve any conflicts, then:
git add .
git commit -m "Update site files"
git push
```

### Step 2 – Deploy to Vercel

**Option A – Automatic (recommended)**

1. Go to https://vercel.com/dashboard
2. Click **Add New → Project**
3. Import the `neilverney4869/Handybloke` GitHub repo
4. Framework Preset: **Other** (it's a static site)
5. Root directory: `/` (leave as default)
6. Click **Deploy**

Vercel will auto-deploy on every push to `main` from now on.

**Option B – Vercel CLI**

```bash
npm i -g vercel
cd /path/to/handybloke
vercel --prod
```

### Step 3 – Connect Custom Domain (optional)

In your Vercel project → **Settings → Domains**, add `thehelpfulbloke.com` and follow the DNS instructions shown.

---

## Making Updates

Edit any `.html` or `.css` file, then:

```bash
git add .
git commit -m "Describe what you changed"
git push
```

Vercel will automatically rebuild and redeploy within ~30 seconds.

---

## Key Details

- **ABN:** 50 751 840 360  
- **WWVP:** 00753390  
- **Phone:** 0490 668 966  
- **Email:** hello@thehelpfulbloke.com  
- **Hours:** Mon–Sat 8am–6pm
