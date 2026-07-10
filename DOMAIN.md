# Custom domain & professional email (P2)

Personal site today: **https://agreyfox.github.io/**  
Product site: **https://agreyfox.github.io/fmr/**

## 1. Custom domain (optional)

Example: `agreyfox.com` or `www.agreyfox.com`.

### DNS (at your registrar)

For **apex** (`agreyfox.com`):

| Type | Name | Value |
|------|------|--------|
| A | `@` | `185.199.108.153` |
| A | `@` | `185.199.109.153` |
| A | `@` | `185.199.110.153` |
| A | `@` | `185.199.111.153` |

For **www**:

| Type | Name | Value |
|------|------|--------|
| CNAME | `www` | `agreyfox.github.io` |

### GitHub

1. Repo `agreyfox.github.io` → **Settings → Pages**
2. Custom domain: enter `agreyfox.com` (or `www.…`)
3. Enable **Enforce HTTPS** after DNS propagates
4. Add a root file `CNAME` containing only the domain (GitHub may create it)

```text
agreyfox.com
```

### After domain is live

- Update `LegalUrls` in the **fmr** Flutter app if product URLs change
- Play Console Website / Privacy → new absolute URLs
- Optional: redirect `agreyfox.github.io` still works as alias

> You must own the domain and set DNS yourself. This file is the checklist only.

## 2. Professional email

Current public contact: **e_raeb@yahoo.com** (works).

More polished options:

| Option | Example | Notes |
|--------|---------|--------|
| Domain mailbox | `hello@agreyfox.com` | Best brand match; use Google Workspace / Fastmail / Cloudflare Email Routing |
| Forwarding | `hello@…` → Yahoo | Cheap; keep Yahoo as inbox |
| Keep Yahoo | `e_raeb@yahoo.com` | Fine for launch; mention on site |

Recommended launch path:

1. Buy domain  
2. Cloudflare Email Routing → forward to Yahoo  
3. Show `hello@agreyfox.com` on profile / case / fmr support  

## 3. One-pager

- Web: https://agreyfox.github.io/case.html  
- PDF: open that page → **Print / Save PDF** (button on page)

## 4. Language

Profile supports **EN / 中文** (nav toggle; preference in `localStorage`).
