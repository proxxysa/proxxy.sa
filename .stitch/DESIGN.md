# Design System: ProxxyMedia
**Project ID:** *(populate after first `create_project` call — update `.stitch/metadata.json`)*

---

## 1. Visual Theme & Atmosphere

ProxxyMedia lives in a world of controlled darkness and electric precision. The aesthetic is **Electric-Dark SaaS** — premium, data-forward, and uncompromisingly modern. Think the control room of a social media war room: deep space blacks, neon-indigo instrument glow, and crisp white readouts.

The interface is **dense-but-breathable**: information is always present, but whitespace is used deliberately to avoid overwhelm. Glassmorphism panels float above the dark canvas, creating subtle depth without distraction. The product should feel like something you *aspire* to use — not just a utility tool, but a command center.

The emotional target: **confident mastery**. Users should feel in control the moment they open a page.

---

## 2. Color Palette & Roles

| Descriptive Name | Hex | Functional Role |
|:---|:---|:---|
| **Deep Obsidian** | `#0A0B14` | Primary page canvas and background |
| **Midnight Slate** | `#12141F` | Card surfaces, panels, sidebar background |
| **Charcoal Lift** | `#1A1C2E` | Hover states on cards, elevated surfaces |
| **Glass Edge** | `rgba(255,255,255,0.06)` | Glassmorphism card borders (1px solid) |
| **Electric Indigo** | `#6C47FF` | Primary actions, active states, brand color |
| **Neon Violet** | `#9B59F5` | Gradient partner to Indigo; secondary highlights |
| **Cyber Cyan** | `#00D4FF` | Sparklines, inline data callouts, icon accents |
| **Mint Success** | `#00E5A0` | Success states, positive metric indicators |
| **Coral Alert** | `#FF4B6E` | Error states, negative trends, alerts |
| **Amber Caution** | `#FFB020` | Warnings, pending states |
| **Pure Cloud White** | `#F0F2FF` | Primary headings and high-emphasis text |
| **Muted Lavender** | `#8B8FA8` | Body copy, secondary labels, placeholder text |
| **Ghost Silver** | `#3A3D52` | Dividers, inactive borders, disabled states |

---

## 3. Typography Rules

- **Font Family:** Inter (Google Fonts) — clean, geometric, highly legible at all sizes
- **Display Headlines (h1):** 64–80px, weight 800 (ExtraBold), letter-spacing -0.03em, Pure Cloud White
- **Section Headlines (h2):** 40–48px, weight 700 (Bold), letter-spacing -0.02em
- **Card Titles (h3):** 20–24px, weight 600 (SemiBold), letter-spacing -0.01em
- **Body Text:** 16px, weight 400 (Regular), line-height 1.7, Muted Lavender on dark backgrounds
- **Labels / Caps:** 11–12px, weight 600, letter-spacing 0.08em, ALL CAPS — used for stat labels and category tags
- **Code / Monospace:** `JetBrains Mono` or `Fira Code` for API keys, code snippets, metric values

---

## 4. Component Stylings

* **Primary Buttons:** Pill-shaped (border-radius: 9999px), Electric Indigo fill (#6C47FF), Pure Cloud White text, 16px semibold. On hover: brightens to Neon Violet (#9B59F5) with a soft indigo glow shadow.

* **Secondary / Ghost Buttons:** Pill-shaped, transparent fill, 1px Electric Indigo border, Electric Indigo text. On hover: Electric Indigo at 10% opacity fill.

* **Cards / Containers:** Midnight Slate (#12141F) background, 1px Glass Edge border (rgba(255,255,255,0.06)), border-radius 16px (generously rounded), whisper-soft diffused box-shadow (0 4px 32px rgba(108,71,255,0.08)). On hover: surface lifts to Charcoal Lift (#1A1C2E) with a faint indigo border glow.

* **Input Fields / Forms:** Midnight Slate background, 1px Ghost Silver border (#3A3D52), border-radius 10px (gently rounded), Muted Lavender placeholder text. On focus: border shifts to Electric Indigo with a soft indigo outer glow ring.

* **Navigation Bar:** Sticky, Deep Obsidian base, glassmorphism blur (backdrop-filter: blur(20px)) on scroll with semi-transparent dark tint. Logo left, links center, CTAs right.

* **Platform Icons (Social):** Monochromatic white by default; animate to their native platform color on hover (Instagram gradient, X white, LinkedIn blue, TikTok neon, etc.).

* **Stat / Metric Cards:** Compact Midnight Slate card, large number in Pure Cloud White (bold), percentage change label in Mint Success (positive) or Coral Alert (negative), small sparkline in Cyber Cyan.

* **Badges / Tags:** Pill-shaped, 8px padding, Electric Indigo background at 15% opacity, Electric Indigo text. "New" badges use Mint Success.

* **Modals / Dialogs:** Midnight Slate surface, 24px border-radius, deep diffused shadow, Electric Indigo close icon, smooth fade+scale entry animation.

---

## 5. Layout Principles

- **Max-Width Container:** 1280px centered, with 48px horizontal padding
- **Whitespace Philosophy:** Generous — sections have 80–120px vertical padding. Cards have 24–32px internal padding.
- **Grid:** 12-column CSS grid at desktop; 2-column at tablet; 1-column at mobile
- **Section Rhythm:** Each major section alternates between full-width dark and slightly elevated card-background sections to create visual breathing room
- **Depth Layering:** Background (Obsidian) → Panels (Midnight Slate) → Cards (Charcoal Lift on hover) → Modals (elevated) — consistent 4-layer elevation system
- **Imagery / Illustrations:** Product screenshots framed in glassmorphism browser-frame mockups with indigo glow behind them. No stock photography.
- **Iconography:** Lucide icons or custom stroke icons — 1.5px stroke weight, 24x24px base size

---

## 6. Design System Notes for Stitch Generation
**Copy this entire block into every baton prompt:**

```
**DESIGN SYSTEM (REQUIRED):**
- Platform: Web, Desktop-first (1440px max-width container)
- Theme: Dark mode — Electric-Dark SaaS aesthetic
- Background: Deep Obsidian (#0A0B14) page canvas; Midnight Slate (#12141F) card/surface
- Primary Accent: Electric Indigo (#6C47FF) — buttons, highlights, active states
- Secondary Accent: Neon Violet (#9B59F5) — gradient partner to indigo
- Highlight: Cyber Cyan (#00D4FF) — data points, sparklines, callouts
- Text Primary: Pure Cloud White (#F0F2FF)
- Text Secondary: Muted Lavender (#8B8FA8)
- Success / Positive: Mint Green (#00E5A0)
- Error / Negative: Coral Alert (#FF4B6E)
- Border: Glass Edge rgba(255,255,255,0.06) 1px
- Font: Inter — 800 display, 700 headings, 600 subheadings, 400 body
- Buttons: Pill-shaped (border-radius 9999px), Electric Indigo fill for primary
- Cards: Glassmorphism — Midnight Slate background, Glass Edge border, 16px radius, soft indigo diffused shadow
- Layout: 1280px max-width, 48px side padding, 12-column grid, generous section whitespace (80–120px vertical)
```
