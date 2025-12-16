# Draw Your Lines — Handoff Document

Generated: 2025-12-15

---

## Current Status

- **Live at:** https://drawyourlines.com/
- **Hosted on:** Netlify (auto-deploys from GitHub on push to `main`)
- **Repo:** https://github.com/virtual-vp/drawyourlines-site
- **Framework:** Hugo 0.152.2 with Ananke theme (via Hugo module)
- **Build status:** Passing (15 pages, ~65ms)

---

## Domains + Canonical Redirects

**Canonical domain:** `https://drawyourlines.com/`

**301 redirects configured in `netlify.toml`:**
- `draw-your-lines.netlify.app` → `drawyourlines.com` (http + https)
- `www.drawyourlines.com` → `drawyourlines.com` (http + https)
- `http://drawyourlines.com` → `https://drawyourlines.com`

---

## Netlify Settings

Configured in `netlify.toml`:

| Setting | Value |
|---------|-------|
| Publish directory | `public` |
| Build command | `hugo --gc --minify --baseURL $URL` |
| Branch | `main` |
| Hugo version | `0.152.2` |
| Go version | `1.22` (for Hugo modules) |
| Deploy previews | Use `$DEPLOY_PRIME_URL` for correct preview URLs |

---

## Site Structure

| Page | URL | File |
|------|-----|------|
| Homepage | `/` | `content/_index.md` |
| Start Here | `/start-here/` | `content/start-here.md` |
| Posts (index) | `/posts/` | `content/posts/_index.md` |
| Now | `/now/` | `content/now.md` |
| About | `/about/` | `content/about.md` |

**Navigation order:** Start Here → Posts → Now → About

---

## Content Inventory

### Pages
| File | Title | Status |
|------|-------|--------|
| `content/_index.md` | Draw Your Lines | Published |
| `content/start-here.md` | Start Here | Published |
| `content/about.md` | About | Published |
| `content/now.md` | Now | Published |
| `content/posts/_index.md` | Posts | Published |

### Posts
| File | Title | Status |
|------|-------|--------|
| `content/posts/the-line.md` | The Line | Published |
| `content/posts/good-enough-is-a-tax.md` | Good Enough Is a Tax | Published |

---

## Assets

| File | Purpose | Size |
|------|---------|------|
| `static/og.png` | Open Graph share image (1200x630) | 692KB |
| `static/favicon.png` | Primary favicon | 55KB |
| `static/favicon.ico` | Legacy favicon fallback | 382B |
| `static/css/custom.css` | Custom styles (nav, hero, pages) | — |

---

## What Changed Today (2025-12-15)

1. Added core pages: Start Here, About, Now, homepage content
2. Created first posts: "The Line", "Good Enough Is a Tax"
3. Homepage redesign: compact navy nav, light hero, no post list
4. Added consistent templates for all pages (baseof, single, list)
5. Netlify config: build settings, Hugo/Go versions
6. Set baseURL to `https://drawyourlines.com/`
7. Added 301 redirects for canonical domain
8. Added favicon (PNG + ICO) and Open Graph image
9. Created curated Posts index page with intro

---

## Next 5 Recommended Tasks

1. **Write 1-2 more posts** — build content momentum before sharing widely
2. **Add RSS feed** — check if Ananke provides one, or add `layouts/_default/rss.xml`
3. **Test social sharing** — paste URL into Twitter/LinkedIn preview tools, verify OG image
4. **Consider analytics** — add Plausible, Fathom, or Netlify Analytics (privacy-respecting)
5. **Plan newsletter/subscribe** — decide if you want email capture (Buttondown, ConvertKit, etc.)

---

## Commands to Run Next Time

```bash
# Navigate to repo
cd ~/Workbox/Web/drawyourlines-site

# Check status
git status
git log --oneline -5

# Start local server
hugo server

# Build for production
hugo --gc --minify

# Push changes
git add . && git commit -m "message" && git push
```

---

## Open Questions / Decisions

### What should the homepage be long-term?
- Current: intro paragraph + 3 curated links
- Options: feature latest post, add visual element, keep minimal

### Should you build a theme/motif system?
- Current: custom CSS with CSS variables (navy, blue, grays)
- Options: formalize color palette, add dark mode toggle, stay minimal

### Add custom domain email or newsletter later?
- Options: Buttondown, ConvertKit, Substack crosspost
- Considerations: ownership vs. convenience, email list portability
- Deferred until content volume justifies it

---

## File Locations Reference

```
~/Workbox/Web/drawyourlines-site/
├── content/
│   ├── _index.md           (homepage)
│   ├── about.md
│   ├── now.md
│   ├── start-here.md
│   └── posts/
│       ├── _index.md       (posts listing)
│       ├── the-line.md
│       └── good-enough-is-a-tax.md
├── layouts/
│   ├── index.html          (homepage template)
│   └── _default/
│       ├── baseof.html     (base template)
│       ├── single.html     (single page/post)
│       └── list.html       (list pages)
├── static/
│   ├── css/custom.css
│   ├── og.png
│   ├── favicon.png
│   └── favicon.ico
├── hugo.yaml               (site config)
└── netlify.toml            (deploy config)
```
