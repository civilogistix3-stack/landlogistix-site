# Land Logistix — Landing Page PRD
**Project:** landlogistix.com landing page  
**Created:** 2026-03-28 | **Owner:** David White  
**Assignee:** Cody  
**Priority:** Build overnight, deploy Monday  
**Status:** Ready for dev

---

## Objective
Build a single-page marketing site at **landlogistix.com** that pre-sells the Land Logistix Skool community. Visitors arrive, understand what they get, and click through to join at **skool.com/landtraining-5514**.

---

## Reference Site
**shippingskool.com** — use as primary design reference.
- Clean, dark background
- Bold typography
- Single CTA that repeats throughout
- Sections: hero → what you get → who it's for → about → pricing → CTA
- No clutter, no navigation menu, no blog sidebar

---

## Tech Stack
- **Pure static HTML/CSS/JS** — single `index.html` file
- **Zero dependencies** — no React, no build tools, no CMS
- **Hosting:** Cloudflare Pages (free tier) — connect to landlogistix.com domain
- **Fonts:** Google Fonts (Inter or similar clean sans-serif)
- **Icons:** Inline SVG or Unicode emoji only — no icon libraries

---

## Design Direction

### Color Palette
- Background: `#0A0F1E` (deep navy/near-black)
- Primary accent: `#F5A623` (warm orange/amber — land/earth feel)
- Secondary accent: `#3B82F6` (blue — trust, expertise)
- Text: `#F8FAFC` (near-white)
- Muted text: `#94A3B8`
- Card backgrounds: `#111827`
- Border: `#1E293B`

### Typography
- Headings: Bold, large, tight line-height
- Body: 16-18px, readable, generous line-height
- Accent text: Orange for emphasis words in headlines

### Tone
- Direct, confident, no fluff
- Speaks to someone who wants to understand the land side of development
- Not "guru" energy — expert practitioner sharing real knowledge

---

## Page Sections

### 1. HERO
**Full-screen, above fold**

```
[LOGO — "LAND LOGISTIX" wordmark, bold, orange X]

[HEADLINE — large, bold, 2 lines max:]
Understand the Land Side
of Real Estate Development

[SUBHEADLINE:]
Most people learn finance and relationships.
Nobody teaches the physical reality of land —
what permits cost, how long entitlements take,
and what kills projects before they start.
Until now.

[CTA BUTTON — large, orange:]
Join the Community →

[SOCIAL PROOF LINE — small text below button:]
Join developers and investors learning the logistics of land
```

---

### 2. THE PROBLEM (no heading — flows from hero)
```
[3 pain points, icon + text format:]

🏗️  You're evaluating sites but don't know what you're really looking at
📋  You're hiring engineers and consultants without knowing if the scope is right
💸  Projects are going over budget and over timeline — and you didn't see it coming
```

---

### 3. WHAT IS LAND LOGISTIX
```
[Section heading:]
What We Teach

[2-column or single column list:]
✅  How land development actually works — start to finish
✅  How to evaluate a site before you buy it
✅  What entitlements are and how to navigate the process
✅  The permitting process — who does what, how long, what it costs
✅  How to hire civil engineers, surveyors, geotech, and attorneys
✅  How to read a site plan, grading plan, and utility layout
✅  Risk management — how to spot the problems that kill projects early
✅  Real deal case studies — what went right, what went wrong

[Below list:]
❌  We don't teach you how to raise capital
❌  We don't teach relationships or deal-making
❌  There are plenty of people who teach that — we teach the land
```

---

### 4. WHO IT'S FOR
```
[Section heading:]
This Is For You If...

[3 cards:]

Card 1:
🏘️  NEW TO DEVELOPMENT
You're exploring commercial or residential real estate and want to understand
the physical side — not just the finance.

Card 2:
📊  ACTIVE INVESTOR
You're already doing deals but realize you don't fully understand
what your engineers are telling you — or how to evaluate their work.

Card 3:
⚙️  CIVIL ENGINEER
You know the technical side. Now you want to understand the
developer's perspective and the business of land.
```

---

### 5. ABOUT DAVID
```
[Section heading:]
Who's Teaching This

[Photo placeholder — left side]
[Text — right side:]

David White, PE
Civil Engineer & Land Developer

David has spent [X] years as a licensed Professional Engineer working on
land development projects across the Southeast — commercial sites, residential
subdivisions, mixed-use, and everything in between.

He's the founder of Civilogistix, a civil engineering firm that has designed
hundreds of projects from raw land to construction documents.

He's not teaching theory. He's teaching what happens on real projects,
what goes wrong, and how to protect yourself before you're too far in to walk away.

[Featured on: "Inside the Blueprint" — logo/text]
```

---

### 6. WHAT'S IN THE COMMUNITY
```
[Section heading:]
What You Get

[Numbered list, styled like shippingskool.com:]

01  A structured curriculum — 8 modules covering the full land development process
02  New content added as David records — grow with the community
03  Community feed — ask questions, share deals, get feedback
04  Track B (add-on) — Technical civil engineering content for engineers
05  Direct access to David and other members who've done the work
06  Risk management frameworks you can apply to your next deal
```

---

### 7. PRICING
```
[Section heading:]
Simple Pricing

[Single pricing card — centered:]

🔒  FOUNDING MEMBER RATE
$[PRICE]/month

✓  Full access to all Land Development Fundamentals content
✓  Community access
✓  New modules as they're released
✓  Your price never increases

[CTA BUTTON:]
Join Land Logistix →
[Small text:] → Takes you to skool.com to complete signup

[Note below:]
The Technical Civil Engineering add-on (Track B) is available separately for engineers.
```

---

### 8. FOOTER CTA (repeat)
```
[Final section:]

If you've ever wished someone would just explain
how the land side of real estate actually works —
this is that place.

[CTA BUTTON:]
Join the Community →

[Footer:]
© 2026 Land Logistix | A Civilogistix Brand
Privacy | Contact
```

---

## CTA Button Behavior
All CTA buttons link to: `https://www.skool.com/landtraining-5514/about`
Open in same tab (not _blank).

---

## Responsive Requirements
- Mobile-first design
- All sections stack cleanly on mobile
- Hero headline scales down gracefully
- CTA buttons are full-width on mobile
- Cards stack vertically on mobile

---

## Logo / Wordmark
- Text-based wordmark: **LAND LOGISTIX**
- The "X" in LOGISTIX styled in orange accent color
- Optional: small icon — abstract "L" or site/land symbol
- No complex graphics needed for launch

---

## Placeholder Content Notes
The following need to be filled in by David before launch:
- [ ] David's professional photo (headshot)
- [ ] Years of experience ("X years")
- [ ] Membership price (TBD — David to confirm)
- [ ] Any testimonials (can launch without)

For now: use placeholder text clearly marked `[PLACEHOLDER]` in the HTML comments.

---

## Deployment Instructions (for Cody)

### Build
1. Single `index.html` file with embedded `<style>` tag
2. All CSS in the `<style>` block — no external CSS file needed for launch
3. No JavaScript required for launch (except optional smooth scroll)

### Deploy to Cloudflare Pages
1. Create repo: `landlogistix-site` on GitHub (civlogistix3-stack org)
2. Push `index.html` to main branch
3. Connect to Cloudflare Pages (free tier)
4. Custom domain: `landlogistix.com`
5. DNS: Add CNAME record at GoDaddy → Cloudflare Pages URL

### GoDaddy DNS Setup
In GoDaddy DNS settings for `landlogistix.com`:
- Type: `CNAME`
- Name: `www`
- Value: `[cloudflare-pages-url].pages.dev`
- For root domain: use Cloudflare nameservers (update nameservers at GoDaddy)

---

## Deliverables
- [ ] `index.html` — complete, responsive, all sections
- [ ] Deployed to Cloudflare Pages
- [ ] landlogistix.com pointing to the page
- [ ] All CTA buttons linking to Skool group
- [ ] Mobile tested

---

*PRD created: 2026-03-28 | Claw / OpenClaw*
