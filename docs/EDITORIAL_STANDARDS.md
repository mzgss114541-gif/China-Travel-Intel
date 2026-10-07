# Editorial Guidelines & Visual Standards

This document establishes the editorial conventions, visual design system tokens, anti-404 source linking standard, and timestamping protocols for published cards.

---

## 1. Anti-404 Source Linking Standard

> [!CAUTION]
> **Never link to fragile single-post deep URLs (`weibo.com/<UID>/<MID>`) or dynamic provincial government CMS subpages.**
> - Single-post status URLs (with post ID suffixes like `/Rl8Jq73wH`) enforce mandatory login walls (SSO) and serve HTTP 404 / visitor redirects to overseas IP addresses and users without active cookies.
> - Government CMS article pages (`.../c100123/2026/content_xxx.shtml`) suffer from rapid permalink decay, archival 404s, or strict WAF firewalls (HTTP 412 / 521 / 403) against non-mainland traffic.

### Standard Rule
The `📌 Primary Source` (EN) and `📌 Fonte Primaria` (IT) hyperlinks must **always point to the verified official entity account profile homepage (`https://weibo.com/u/<UID>`)**, or the verified official root portal:
- **Strip Single-Post Suffixes**: Transform `https://weibo.com/<UID>/<MID>` ➔ `https://weibo.com/u/<UID>`.
- **Anchor Text Convention**:
  - English: `[Authority Name] (Sina Weibo)` or `[Authority Name] (Official Portal)`
  - Italian: `[Nome Autorità] (Sina Weibo)` or `[Nome Autorità] (Portale Ufficiale)`

---

## 2. CST Timestamping & Verification Banner Standard

- **Timestamp Badge**: The badge on every dispatch card must strictly display authentic China Standard Time (`HH:MM CST`, e.g., `09:15 CST`, `14:30 CST`).
- **Verification Cycle Banner**: Must strictly read:
  - English: `<strong style="color: #2c2825;">Verification Cycle:</strong> Daily Purified (October 2026)`
  - Italian: `<strong style="color: #2c2825;">Ciclo di Verifica:</strong> Aggiornamento Giornaliero (Ottobre 2026)`

---

## 3. Visual Design System Tokens

- **Card Background**: `#faf8f5` (Warm Alabaster)
- **Card Border**: `1px solid #ede8e1` / `1px solid rgba(140, 115, 85, 0.25)` (Refined Bronze Accent)
- **Card Shadow**: `0 2px 10px rgba(44, 40, 37, 0.03)`
- **Header Font**: `'Cinzel', 'Playfair Display', Georgia, serif` (`#2c2825`, 18px, font-weight 700)
- **Body Font**: `'Montserrat', 'Inter', -apple-system, sans-serif` (`#524b45`, 15px, line-height 1.75)
- **Category Badge**: Background `#f4ede4`, Text `#785a36`, 11px uppercase, font-weight 700.
- **Timestamp Badge**: Background `#8c7355`, Text `#ffffff`, 12px, font-weight 600.
- **Primary Source Link**: Color `#8c7355`, text-decoration underline, font-weight 600.
