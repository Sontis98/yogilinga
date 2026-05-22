# Yogi & Linga — yogilinga.com

Sexual wellness editorial blog targeting the US market (25–34, Millennials & Gen Z).

## Stack

- **Jekyll** — static site generator
- **GitHub Pages** — free hosting, auto-deploy
- **Cloudflare** — CDN, HTTPS, DDoS protection (add after GitHub Pages setup)

---

## Local Development

### 1. Install dependencies

```bash
gem install bundler
bundle install
```

### 2. Run locally

```bash
bundle exec jekyll serve --livereload
```

Open [http://localhost:4000](http://localhost:4000)

---

## Deploy to GitHub Pages

### One-time setup

1. Create a new GitHub repository named `yogilinga` (or any name)
2. Go to **Settings → Pages → Source** → select **GitHub Actions**
3. Push your code:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/yogilinga.git
git push -u origin main
```

The GitHub Action in `.github/workflows/deploy.yml` auto-builds and deploys on every push to `main`.

### Custom domain (yogilinga.com)

1. In your repo, go to **Settings → Pages → Custom domain**
2. Enter `yogilinga.com` and save
3. This creates a `CNAME` file automatically
4. In your DNS provider (Cloudflare recommended), add:

```
A     @     185.199.108.153
A     @     185.199.109.153
A     @     185.199.110.153
A     @     185.199.111.153
CNAME www   YOUR_USERNAME.github.io
```

---

## Adding Content

### Add a product review

Create `_reviews/product-name.md`:

```yaml
---
layout: review
title: "Product Name Review: Is It Worth It?"
date: 2025-06-01
category: "vibrator"
brand: "Brand Name"
product_name: "Product Name"
score: 8.5
price: "$129"
buy_url: "https://your-affiliate-link.com"
affiliate: true
scores:
  - name: "Motor Strength"
    value: 8.5
  - name: "App Quality"
    value: 7.0
  - name: "Material Safety"
    value: 10.0
  - name: "Noise Level"
    value: 9.0
  - name: "Battery Life"
    value: 8.0
  - name: "Value for Money"
    value: 8.5
excerpt: "One sentence summary for SEO and cards."
---

Your review content here in Markdown.
```

### Add a wellness/editorial post

Create `_posts/YYYY-MM-DD-post-title.md`:

```yaml
---
layout: post
title: "Your Article Title"
date: 2025-06-01
category: "wellness"
read_time: 8
affiliate: false
excerpt: "One sentence for SEO."
tags: [neuroscience, sleep, stress-relief]
---

Article content in Markdown.
```

---

## Affiliate Networks to Join

| Network | Brands | Commission |
|---------|--------|------------|
| ShareASale | Lovehoney, Adam & Eve | 15–20% |
| Awin | We-Vibe, Womanizer | 15–20% |
| LELO Direct | LELO | 20–25% |

**FTC requirement:** All review posts with affiliate links must have `affiliate: true` in frontmatter — this auto-displays the disclosure banner.

---

## Legal Checklist (US Market)

- [x] Age gate on every page
- [x] Affiliate Disclosure page at `/affiliate-disclosure/`
- [ ] Privacy Policy at `/privacy/` — add before launch
- [ ] Terms of Use at `/terms/` — add before launch
- [x] `rel="nofollow sponsored"` on all affiliate links
- [x] "For adults 18+ only" in footer
