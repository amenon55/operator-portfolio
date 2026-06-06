# Operator Portfolio — Claude Context

## What this project is

Single-page personal portfolio site for Abi Menon at **abimenon.com**. Positions as a PE portfolio company operator: M&A integration, turnaround, Lean execution, AI-enabled ops.

## Tech stack

- Pure HTML5 / CSS / vanilla JS — no framework, no build step, no npm
- Based on HTML5 UP "Read Only" template, heavily customized
- Hosted on **GitHub Pages** — push to `main` deploys automatically
- `CNAME` file → `abimenon.com`

## File structure

```
index.html          — entire site (~2,100 lines, includes all embedded CSS)
assets/css/         — base template stylesheets
assets/js/          — JS for nav, lightbox, counter animations
images/             — headshots, case screenshots, playbook screenshots
documents/          — PDFs linked from playbook and "up to speed" sections
docs/               — session summaries and task tracking (not served)
CNAME               — GitHub Pages custom domain
sitemap.xml
robots.txt
```

## Site sections (in nav order)

| ID | Nav label | Content |
|---|---|---|
| `#one` | Overview | Hero: title, lead copy, 4 bullet list, metrics row ($50M P&L, 150 headcount, 10 turnarounds), Operator Snapshot panel |
| `#speed` | Up to speed fast | "Operator Ramp System" — 3-page PDF thumbnails with lightbox viewer |
| `#two` | Selected Operating Work | 4 case cards (image-based): Asset Portfolio Recovery $25M, Industrial Turnaround $25M, Saving the Integration (Covid), Regulatory Discipline (NIOSH) |
| `#three` | Automation I've Deployed | n8n + Cursor invoice automation case; n8n task management case |
| `#four` | Integration Playbook | PDF thumbnails: Governance, Operations Checklist, EBITDA Dashboard, Synergy Tracker, Integration Timeline |
| `#five` | Media | Apple Podcasts embed — Workforce One podcast |
| `#six` | Personal | Photo grid: Cold Plunge, Salsa Dancing, Yoga, Toastmasters, BJJ |
| `#seven` | Contact | Email, LinkedIn, Zoom booking buttons |

## How to edit

Everything is in `index.html`. CSS is embedded in `<style>` tags in the `<head>`. No build required — edit and push.

**Deploy:** `git add index.html && git commit -m "..." && git push` → live in ~30 seconds.

## Key CSS variables

```css
--navy: #061B49;
--navy-dark: #031234;
```

## Conventions

- Comments in code are minimal — use section IDs to navigate
- Images: `loading="lazy" decoding="async"` on all non-hero images
- PDFs open in a custom lightbox (`class="playbook-pdf-open"`, `data-pdf-src`)
- Metric counters animate on scroll via JS (`data-metric-end` attribute)

## Session docs

- `docs/SESSION_SUMMARY.md` — current state of the site and recent changes
- `docs/TASKS.md` — next concrete task only
