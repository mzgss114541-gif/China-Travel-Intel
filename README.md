# China-Travel-Intel

> **Official Inbound Travel Intelligence & Luxury Editorial Knowledge Base for China**  
> Serving [YouTu Travel](https://yoututravel.com) — Dual-language (English & Italian) independent and bespoke travel portal for international travelers entering China.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Status: Production](https://img.shields.io/badge/Status-Production-success.svg)]()
[![Languages: EN | IT](https://img.shields.io/badge/Languages-EN%20%7C%20IT-gold.svg)]()

---

## 📖 Overview

**China-Travel-Intel** is the centralized content repository and architectural blueprint powering the travel intelligence and editorial guides for **YouTu Travel** ([yoututravel.com](https://yoututravel.com)).

This repository maintains version-controlled editorial assets in structured Markdown format, covering:
1. **Long-Form Pillar Guides**: In-depth, high-converting pillar content on independent travel in China.
2. **Living Regional Intelligence Hubs**: Chronological, verified travel dispatches across the **5 Canonical Regional Hubs** in both **English** and **Italian**.
3. **Core Site Pages**: Brand philosophy, custom trip planning, and guide pages.
4. **Editorial & Architectural Documentation**: Full specifications of the ingestion crawlers, the Inbound Luxury Filter, the Anti-404 source linking standard, and the 5-Hub regional matrix.

---

## 🗂️ Content Directory Structure

```text
China-Travel-Intel/
├── README.md                           # Main repository overview & implementation guide
├── docs/                               # Architecture and editorial specifications
│   ├── ARCHITECTURE.md                 # Pipeline architecture & ingestion implementation
│   ├── CONTENT_CURATION.md             # The Inbound Luxury Filter (inclusions & blacklist)
│   ├── EDITORIAL_STANDARDS.md          # Anti-404 standard, CST timestamping & styling tokens
│   └── REGIONAL_HUBS_MATRIX.md         # The 5 canonical regional hubs mapping
├── content/
│   ├── blog/                           # Long-form pillar guides
│   │   └── en/
│   │       └── independent-travel-china-guide.md
│   ├── intelligence-hubs/              # The 5 Canonical Regional Hubs (Bilingual)
│   │   ├── en/                         # English Hubs
│   │   │   ├── national-policy-transit.md      (Post ID: 1227)
│   │   │   ├── west-china.md                   (Post ID: 1243)
│   │   │   ├── east-china.md                   (Post ID: 1252)
│   │   │   ├── south-china.md                  (Post ID: 1256)
│   │   │   └── north-china.md                  (Post ID: 1258)
│   │   └── it/                         # Italian Hubs
│   │       ├── national-policy-transit.md      (Post ID: 1228)
│   │       ├── west-china.md                   (Post ID: 1244)
│   │       ├── east-china.md                   (Post ID: 1253)
│   │       ├── south-china.md                  (Post ID: 1257)
│   │       └── north-china.md                  (Post ID: 1259)
│   └── pages/                          # Core website pages
│       ├── en/                         # English pages (About Us, Planning, Contact, Privacy)
│       └── it/                         # Italian pages (Chi siamo, Pianificazione, Contatta, etc.)
```

---

## 🧭 Live Content Inventory

### 1. Long-Form Pillar Guides
| Lang | Post ID | Title | Slug | Topic |
|:---:|:---:|:---|:---|:---|
| 🇬🇧 EN | `1094` | Independent Travel China: Do You Really Need a Group Tour? | `independent-travel-china-guide` | Comprehensive guide on navigating China autonomously without 40-person tour buses |

### 2. The 5 Regional Intelligence Hubs (Bilingual)
| Hub Code | Coverage / Key Destinations | 🇬🇧 English Hub | 🇮🇹 Italian Hub |
|:---|:---|:---:|:---:|
| `National_Policy_Transit` | 15/30-day visa exemptions, 144-Hour TWOV, customs, CAAC corridors, 12306 rail booking | [ID 1227](content/intelligence-hubs/en/national-policy-transit.md) | [ID 1228](content/intelligence-hubs/it/national-policy-transit.md) |
| `West_China` | Xi'an, Chengdu, Jiuzhaigou, Yunnan, Tibet, Xinjiang (Silk Road), Dunhuang | [ID 1243](content/intelligence-hubs/en/west-china.md) | [ID 1244](content/intelligence-hubs/it/west-china.md) |
| `East_China` | Shanghai, Suzhou, Hangzhou, Huangshan, Jingdezhen, Shandong, Fujian | [ID 1252](content/intelligence-hubs/en/east-china.md) | [ID 1253](content/intelligence-hubs/it/east-china.md) |
| `South_China` | Guangzhou, Shenzhen (GBA), Guilin, Yangshuo, Sanya, Zhangjiajie, Three Gorges | [ID 1256](content/intelligence-hubs/en/south-china.md) | [ID 1257](content/intelligence-hubs/it/south-china.md) |
| `North_China` | Beijing (Forbidden City, Great Wall), Tianjin, Shanxi (Datong/Pingyao), Luoyang, Harbin | [ID 1258](content/intelligence-hubs/en/north-china.md) | [ID 1259](content/intelligence-hubs/it/north-china.md) |

---

## ⚙️ System Implementation & Architecture

The content in this repository is powered by a multi-tier intelligence pipeline operating continuously in the background:

### 1. Zero-Cookie Ingestion Suite
- **Monitoring Scope**: Tracks 36+ provincial culture & tourism departments, national museums, CAAC civil aviation bulletins, and China State Railway Group (12306).
- **Architecture**: Multi-threaded Python scrapers operating with zero-cookie headers, bypassing anti-scraping blocks and feeding into a self-hosted FreshRSS engine via structured OPML registries.

### 2. The Inbound Luxury Filter
- **Filtering Logic**: Incoming notices are filtered to eliminate domestic trivia (petty border smuggling, conductor lost-item notices, local marathons, internal administrative cadre meetings).
- **High-Impact Retention**: Preserves only operational intelligence directly affecting affluent international visitors: ticket quota warnings, passport reservation windows, high-altitude alpine weather closures, and visa-free policies.
- Detailed criteria: [`docs/CONTENT_CURATION.md`](docs/CONTENT_CURATION.md).

### 3. The Anti-404 Source Linking Standard
- Chinese social media (Weibo) single-post URLs enforce mandatory login walls (SSO) and serve HTTP 404 / visitor redirects to overseas IP addresses.
- All primary source links are transformed to point strictly to **verified entity account profiles** (`https://weibo.com/u/<UID>`) or official government root domains.
- Detailed standard: [`docs/EDITORIAL_STANDARDS.md`](docs/EDITORIAL_STANDARDS.md).

### 4. Dual-Language Synthesis & Publishing
- Dispatches are synthesized into parallel **English** and **Italian** cards.
- Each dispatch features authentic **China Standard Time (`HH:MM CST`)** timestamp badges and daily verification headers.
- Deployed headlessly to WordPress production hubs via CLI workflows with automated cache flushing.

---

## 📄 License & Attribution

Content copyright &copy; [YouTu Travel](https://yoututravel.com). All rights reserved.  
Technical documentation and editorial standards licensed under the [MIT License](LICENSE).
