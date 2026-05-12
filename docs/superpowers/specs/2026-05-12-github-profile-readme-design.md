# GitHub Profile README — Design Spec
**Date:** 2026-05-12
**Author:** Vivek Jivani
**File target:** `README.md` (root of `vivekjivani/vivekjivani` GitHub profile repo)

---

## Overview

A story-driven, friendly GitHub profile README for Vivek Jivani — Full Stack Engineer & Architect. Primary goal: attract freelance clients and full-time employers. Tone: warm and approachable. The reader should feel like they're meeting a real, capable person, not scanning a CV.

---

## Section 1 — Header & About Me

### Header
- Wave emoji 👋 rendered as plain text (GitHub strips CSS animations — no actual animation on the emoji)
- Animated gradient heading: use `readme-typing-svg.demolab.com` to generate an SVG `<img>` tag that displays "Hey, I'm Vivek Jivani" with a typewriter animation. Color: `#58a6ff`. This is a single-color animated SVG — the multi-color gradient effect from the mockup is a design-only reference and will be approximated by the typed color.
- Subtitle: `Full Stack Engineer & Architect · Surat, India 🇮🇳`
- Three status badges (shields.io static badges):
  - `⚡ Open to Freelance` (blue)
  - `✅ Available Now` (green)
  - `🌍 Remote Worldwide` (purple)
- One-liner tagline: *"I build things that actually work — end-to-end products from design to deployment, across web and mobile."*
- Social links row (icon + text, inline): Portfolio · LinkedIn · Email

### About Me
Four info cards rendered as an HTML table (2×2 grid using `<img>` spacer trick or aligned markdown):
1. 🏗️ 6+ years shipping production apps — from B2B diamond trading platforms to cloud-native data tools
2. 📱 Comfortable across Flutter mobile and Next.js / React web — one engineer, full product
3. 🤖 AI-powered workflow — uses Claude & Gemini daily for architecture, code review, and debugging
4. 🚀 Last big win: architected a serverless platform that delivered a 70% productivity boost at Nexsales

**Implementation note:** GitHub README doesn't support CSS grid. Use an HTML `<table>` with two columns, or aligned `<div>` blocks. Test rendering on github.com.

---

## Section 2 — Tech Stack

Grouped badges using [shields.io](https://shields.io) `?logo=` and `?style=for-the-badge` style. No React Native.

| Group | Technologies |
|---|---|
| 📱 Mobile | Flutter |
| 🌐 Frontend | Next.js, React, TypeScript, JavaScript |
| ⚙️ Backend | Node.js, Firebase |
| 🗄️ Databases | PostgreSQL, MongoDB, Redis |
| ☁️ DevOps & Cloud | Docker, Google Cloud, GitHub Actions |
| 🤖 AI Tools | Claude, Gemini |

Each badge uses `shields.io/badge/` with matching brand colors and logos.

---

## Section 3 — Featured Projects

Six projects in a 2×3 layout. GitHub markdown doesn't support CSS grid — use an HTML `<table>` with two columns, each cell containing project info. Each project has:
- Emoji icon + name (bold)
- Type label (italic, small)
- 2-sentence description
- Tech tags (inline code or small badges)
- Live/store link where applicable

| Project | Type | Key detail | Link |
|---|---|---|---|
| ⚡ Goldmine | Data Automation Platform | 70% productivity boost, 60% cost reduction | — |
| 💎 Craft Diamonds | Flutter iOS/Android App | B2B diamond trading, Play Store | Play Store |
| 📞 VoiceReach Dialer | Cloud Sales Platform | Docker microservices architecture | voicereach.us |
| 🧾 GST Tools | Flutter Tax Utility App | Offline-first, Play Store | Play Store |
| 🌸 Reiki Surat | Freelance Website | Wellness center, calming design | reikisurat.in |
| 🦷 Varni Dental Care | Freelance Website | Dental clinic, patient-friendly UX | varnidentalcare.in |

---

## Section 4 — GitHub Stats + Contact

### GitHub Stats
Three widgets from [github-readme-stats](https://github.com/anuraghazra/github-readme-stats), displayed side by side using an HTML table:
1. **Overall stats card** — `github-readme-stats.vercel.app/api?username=vivekjivani&show_icons=true&theme=github_dark`
2. **Streak stats** — `github-readme-streak-stats.herokuapp.com/?user=vivekjivani&theme=github-dark-blue`
3. **Top languages** — `github-readme-stats.vercel.app/api/top-langs/?username=vivekjivani&layout=compact&theme=github_dark`

### Contact / Let's Work Together
Three cards (HTML table, 3 columns):
- 🌐 Portfolio — vivekjivani.com
- 💼 LinkedIn — linkedin.com/in/vivekjivani
- 📧 Email — vivekjivani17@gmail.com

### Footer
- Centered text: *"Open to freelance projects and full-time roles — remote worldwide 🌍"*
- Light human touch: *"⚡ Powered by coffee, curiosity, and a solid Wi-Fi connection"*
- Optional: visitor counter badge (shields.io visitor badge)

---

## Technical Constraints

- GitHub profile README renders GitHub Flavored Markdown (GFM) — no `<style>` tags, no CSS classes, no JavaScript
- Layout tricks must use HTML `<table>`, `<img>` width spacers, and `align` attributes
- All external images (badges, stats widgets) must be hotlinked — no local images
- Shields.io badges: use `style=for-the-badge` for visual weight
- Stats widgets: `theme=github_dark` to match GitHub's dark mode
- Animated typing header: use `readme-typing-svg.demolab.com` for the name typewriter effect

---

## Success Criteria

- Loads cleanly on github.com/vivekjivani in both light and dark mode
- All links are clickable and point to correct destinations
- Stats widgets load (may need a few seconds on first visit)
- Visitor feels the friendly-professional tone within 5 seconds of scanning
- Clear call to action for freelance/hiring visible without scrolling
