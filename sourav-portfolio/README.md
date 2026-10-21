# Sourav Pati – Portfolio

A single-page static portfolio. No build step, no dependencies.

## Files
- `index.html` – the whole site (HTML, CSS, JavaScript)
- `vercel.json` – Vercel settings (clean URLs, basic security headers)

## Preview locally
Open `index.html` in a browser, or from this folder run:

    python3 -m http.server 8000

then visit http://localhost:8000

## Deploy to Vercel

### Option A: Vercel CLI (fastest)
1. Install Node.js, then run `npm i -g vercel`
2. In this folder run `vercel` and answer the prompts:
   - Set up and deploy? **Y**
   - Link to existing project? **N**
   - Directory containing your code? **./**
   - Override settings? **N**
3. Run `vercel --prod` to publish to your production URL.

### Option B: GitHub + Vercel dashboard (auto-deploys on every push)
1. Create a new GitHub repo and push this folder:

       git init
       git add .
       git commit -m "Add portfolio"
       git branch -M main
       git remote add origin https://github.com/spati10/portfolio.git
       git push -u origin main

2. Go to vercel.com/new and import the repo.
3. Framework Preset: **Other**. Leave Build Command and Output Directory empty.
4. Click **Deploy**.

### Custom domain (optional)
Vercel dashboard → your project → Settings → Domains → add your domain and follow the DNS steps.

## Editing
Update text directly in `index.html`: search for the project names, email, or links. Push (Option B) or run `vercel --prod` (Option A) to publish changes.
