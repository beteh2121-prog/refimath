# RefiMath — Mortgage Refinance Calculator Site

Free mortgage refinance break-even calculator + blog. Deployed via GitHub + Netlify.

## 🗂️ Folder Structure

```
refimath/
│
├── index.html                          ← Main calculator (homepage)
├── blog.html                           ← Blog index
├── about.html                          ← About page (AdSense required)
├── privacy.html                        ← Privacy policy (AdSense required)
├── 404.html                            ← Custom error page
├── sitemap.xml                         ← Submit to Google Search Console
├── robots.txt                          ← Crawler rules
├── _redirects                          ← Netlify redirects config
│
├── .devcontainer/
│   └── devcontainer.json               ← Auto-configures Codespaces perfectly
│
├── .github/
│   └── workflows/
│       └── notify-search-engines.yml   ← Auto-pings Google/Bing on every push
│
├── assets/
│   └── css/
│       └── shared.css                  ← Shared styles for all pages
│
└── blog/
    ├── is-it-worth-refinancing-2026.html
    ├── refinancing-closing-costs-2026.html
    └── how-long-break-even-refinance.html
```

---

## 🚀 Deploy via GitHub Codespaces (Recommended)

### First-time setup

1. Create a new **public** repo on github.com named `refimath`
2. Go to the repo → green **Code** button → **Codespaces** tab → **Create codespace on main**
3. Wait ~30 seconds for Codespaces to open (VS Code in your browser)
4. In the Explorer panel, drag all files from this zip into the Codespaces window
5. In the terminal at the bottom, run:

```bash
git add .
git commit -m "Initial site launch"
git push
```

6. Connect Netlify to your GitHub repo (netlify.com → Add new site → Import from GitHub)
7. Netlify auto-deploys every time you push. **Stop your Codespace when done.**

---

## ✍️ How to Add a New Blog Post (weekly routine)

1. Open your Codespace at github.com/codespaces
2. Right-click `blog/is-it-worth-refinancing-2026.html` → Copy → Paste → rename to your slug
3. Edit the new file — update title, description, canonical URL, h1, date, and article content
4. Add a card to `blog.html` (copy the template comment block)
5. Add a URL entry to `sitemap.xml`
6. In terminal:

```bash
git add .
git commit -m "Blog: Your Post Title Here"
git push
```

7. Stop your Codespace → go to Google Search Console → request indexing of new URL

---

## 💰 Monetization Checklist

- [ ] Replace `ca-pub-XXXXXXXXXXXXXXXX` with your AdSense publisher ID in ALL html files
- [ ] Replace affiliate href links in index.html with real LendingTree/Credible affiliate URLs
- [ ] Update `refimath.com` in sitemap.xml and canonical tags to your real domain
- [ ] Update `hello@refimath.com` in about.html and privacy.html
- [ ] Add Google Analytics GA4 script to all pages

---

## 💡 Next 8 Blog Posts to Write (sorted by easiest to rank)

| Post title | KD | CPC | Searches/mo |
|---|---|---|---|
| How to negotiate lower closing costs | ~19 | $22 | 2,900 |
| No-closing-cost refinance: is it worth it? | ~21 | $25 | 2,400 |
| VA IRRRL streamline refinance guide | ~24 | $18 | 3,600 |
| Should I refinance to a 15-year mortgage? | ~22 | $28 | 3,200 |
| What credit score do you need to refinance? | ~28 | $31 | 5,400 |
| FHA streamline refinance: who qualifies? | ~27 | $22 | 4,100 |
| Cash-out refinance vs home equity loan | ~31 | $35 | 6,600 |
| ARM vs fixed rate mortgage 2026 | ~35 | $29 | 8,100 |

---

## ⚡ Save Your Free Codespaces Hours

- **Always stop** the codespace when done: `Ctrl+Shift+P` → "Stop Current Codespace"
- Set idle timeout to **5 minutes**: github.com → Settings → Codespaces → Default idle timeout
- Use **2-core machine** only (default) — 4-core uses hours twice as fast
- For small edits, use **github.dev** instead: press `.` on your repo page (zero hours used)
- Free tier = ~60 real hours/month on 2-core. A content site needs ~3–5 hrs/month
