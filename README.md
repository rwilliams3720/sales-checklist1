# Sales Submission Checklist

A dynamic, interactive sales submission checklist web app. Enter sale quantities and rows generate automatically in the detail table.

## Features

- Submission date (auto-filled to today) and customer name
- Forms checklist: GSD, DSS, SCD, SFPP — each with submitted checkbox, customer notified checkbox, and notification date
- Sale type counters: Auto, Fire, Health, Life — dynamically generate detail rows
- Detail table with Desc, Premium, and Period columns grouped by sale type
- Print / Save as PDF via browser
- Clear form button
- Fully responsive

## Local Development

No build step needed — it's a single HTML file.

```bash
# Just open in browser
open index.html

# Or serve locally with any static server, e.g.:
npx serve .
```

## Deploy to Vercel via GitHub

### Step 1 — Create a GitHub repository

1. Go to [github.com](https://github.com) and sign in (or create a free account)
2. Click the **+** icon (top right) → **New repository**
3. Name it something like `sales-checklist`
4. Set it to **Public** or **Private** (both work with Vercel)
5. Click **Create repository**

### Step 2 — Upload your files to GitHub

**Option A — GitHub web interface (no Git required):**
1. On your new repo page, click **Add file → Upload files**
2. Drag and drop both `index.html` and `vercel.json`
3. Click **Commit changes**

**Option B — Git command line:**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/sales-checklist.git
git push -u origin main
```

### Step 3 — Deploy to Vercel

1. Go to [vercel.com](https://vercel.com) and sign in with your GitHub account
2. Click **Add New → Project**
3. Find your `sales-checklist` repo and click **Import**
4. Leave all settings as default — Vercel will detect the static site automatically
5. Click **Deploy**

That's it! Vercel will give you a live URL like:
`https://sales-checklist-yourname.vercel.app`

### Step 4 — Future updates

Any time you push a change to GitHub, Vercel automatically redeploys within ~30 seconds.

```bash
# Make your edits to index.html, then:
git add .
git commit -m "Update checklist"
git push
```

## Custom Domain (Optional)

1. In your Vercel project dashboard, go to **Settings → Domains**
2. Add your domain and follow the DNS instructions

## Files

| File | Purpose |
|------|---------|
| `index.html` | The entire app — all HTML, CSS, and JavaScript |
| `vercel.json` | Vercel deployment configuration |
| `README.md` | This file |
