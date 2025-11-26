# Polite Chaos

> A creative studio portfolio that blends clean typography with playful motion — built with Next.js 15, GSAP, and Lenis.

![Next.js](https://img.shields.io/badge/Next.js-15-black?logo=next.js)
![React](https://img.shields.io/badge/React-19-61DAFB?logo=react)
![GSAP](https://img.shields.io/badge/GSAP-3.13-88CE02?logo=greensock)
![License](https://img.shields.io/badge/License-MIT-blue)

---

## ✨ Overview

Polite Chaos showcases featured projects, client stories, studio info, and contact details through:

- Cinematic preloader & hero animations
- Smooth scroll (Lenis) + scroll-triggered effects (GSAP ScrollTrigger)
- Page transitions via `next-view-transitions`
- A showreel experience backed by custom media & music

---

## 🛠 Tech Stack

| Category  | Tools                                                          |
| --------- | -------------------------------------------------------------- |
| Framework | Next.js 15 (App Router)                                        |
| UI        | React 19, CSS (global + component-level)                       |
| Animation | GSAP, ScrollTrigger, @gsap/react, Lenis, next-view-transitions |
| Utilities | react-icons, split-type                                        |
| Fonts     | Neue Montreal, Big Shoulders Display, Pangram Sans, Geist Mono |

---

## 🚀 Quick Start

```bash
# 1. Install dependencies (pnpm recommended)
pnpm install

# 2. Start dev server
pnpm dev
```

Open **http://localhost:3000** — edits hot-reload automatically.

### Production

```bash
pnpm build   # optimized build
pnpm start   # run production server
```

---

## 📁 Project Structure

```
src/
├─ app/
│  ├─ layout.js          # Root layout + ViewTransitions
│  ├─ page.jsx           # Home (hero, showreel, featured work, reviews, spotlight, CTA, footer)
│  ├─ studio/            # Studio page
│  ├─ work/              # Work gallery
│  ├─ stories/           # Story slides
│  ├─ contact/           # Contact form
│  └─ sample-project/    # Single project detail
├─ components/
│  ├─ Preloader/         # Timed entrance animations
│  ├─ Showreel/          # Video/image reel
│  ├─ FeaturedWork/      # Portfolio grid (project.js)
│  ├─ ClientReviews/     # Testimonials (clientReviewsData.js)
│  ├─ Spotlight/         # Highlighted stories
│  ├─ StorySlides/       # Story slider (stories.js)
│  ├─ TeamCards/         # Team members (teamMembers.js)
│  └─ Button/, Copy/, CTACard/, Footer/, Menu/
└─ hooks/
   └─ useViewTransition.js

public/
├─ featured-work/, work/, project/, spotlight/, stories/, team-cards/, showreel/, studio/
├─ fonts/                # Custom typefaces
└─ site-logo.png, logo.svg
```

---

## 🎨 Customization

| What                      | Where                                                                                           |
| ------------------------- | ----------------------------------------------------------------------------------------------- |
| Hero copy & CTAs          | `src/app/page.jsx`                                                                              |
| Section titles            | Route components (`studio/page.jsx`, etc.)                                                      |
| Projects / Stories / Team | Data files in components (`project.js`, `stories.js`, `teamMembers.js`, `clientReviewsData.js`) |
| Global styles             | `src/app/globals.css`                                                                           |
| Route styles              | `home.css`, `studio.css`, `work.css`, etc.                                                      |
| Fonts                     | `public/fonts/` + `src/app/fonts.css`                                                           |
| Branding                  | `public/site-logo.png`, `public/logo.svg`, update refs in `layout.js`                           |

---

## 🌐 Deployment

Deploy anywhere that supports Next.js 15:

- **Vercel** (recommended) — zero-config deploy
- **Custom Node server** — `pnpm build && pnpm start`
- **Docker / serverless** — follow Next.js docs

---

## 📄 License

MIT © Akmal
