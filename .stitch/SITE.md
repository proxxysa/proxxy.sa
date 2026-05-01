# Project Vision & Constitution
> **AGENT INSTRUCTION:** Read this file before every iteration. It serves as the project's "Long-Term Memory."

## 1. Core Identity
* **Project Name:** ProxxyMedia
* **Stitch Project ID:** *(populate after `create_project`)*
* **Domain:** proxxymedia.com
* **Mission:** A premium social media account management platform that lets agencies, creators, and brands manage every account, schedule every post, and measure every result — from one unified workspace.
* **Target Audience:** Social media agencies, content creators, marketing teams, and brand managers handling multiple social accounts across platforms (Instagram, X/Twitter, LinkedIn, TikTok, Facebook, Pinterest, YouTube).
* **Voice:** Confident, intelligent, and efficient. Never corporate-stiff. Premium without being cold.

---

## 2. Visual Language
*Reference these descriptors when prompting Stitch.*

* **The "Vibe" (Adjectives):**
    * *Primary:* Electric-Dark — deep obsidian backgrounds, high-contrast neon-indigo accents, glassmorphism cards
    * *Secondary:* Premium SaaS — data-dense but breathable, structured whitespace, clear information hierarchy
    * *Tertiary:* Confident & Fluid — pill-shaped actions, smooth micro-animations, no visual noise

* **Atmosphere Summary for Stitch Prompts:**
  > "A premium dark-mode SaaS dashboard with electric indigo accents (#6C47FF) on deep obsidian backgrounds (#0A0B14). Glassmorphism cards with subtle violet-tinted borders. Bold Inter typography. Pill-shaped primary buttons. Clean data visualization with glowing accent lines."

---

## 3. Architecture & File Structure
* **Root:** `site/public/`
* **Stitch Staging:** `.stitch/designs/` → validate → move to `site/public/`
* **Metadata:** `.stitch/metadata.json` (Stitch project + screen IDs — persist!)
* **Design Source:** `.stitch/DESIGN.md` (copy Section 6 block into every baton)
* **Navigation Strategy:** Sticky top nav with ProxxyMedia logo (left), main links (center), and CTA/avatar (right). All pages share this nav and a minimal footer.

---

## 4. Live Sitemap (Current State)
*Update with `[x]` when a page is successfully generated and merged.*

* [ ] `index.html` — Marketing landing page: hero, feature highlights, social proof, pricing teaser, CTA
* [ ] `dashboard.html` — Main app dashboard: KPI cards, quick-compose, recent posts, account health overview
* [ ] `accounts.html` — Connected accounts manager: add/remove platforms, health status, permission controls
* [ ] `scheduler.html` — Content calendar: monthly/weekly view, drag-and-drop scheduling, post queue
* [ ] `composer.html` — Post creation studio: rich editor, multi-platform preview, media upload, AI assist
* [ ] `analytics.html` — Performance analytics: reach/engagement/follower growth charts, post performance table
* [ ] `inbox.html` — Unified inbox: comments, DMs, mentions across all connected accounts
* [ ] `reports.html` — Custom reports builder: template library, export to PDF/CSV
* [ ] `pricing.html` — Pricing plans: Starter / Pro / Agency tiers, feature comparison table
* [ ] `login.html` — Authentication: login, sign up, OAuth social login options
* [ ] `onboarding.html` — Onboarding flow: connect first account, platform picker, welcome checklist
* [ ] `settings.html` — Account settings: profile, team members, integrations, billing, API keys

---

## 5. The Roadmap (Backlog)
*Pick the next task from here if available.*

### High Priority (Core App)
- [ ] `dashboard.html` — Build after `index.html`; establishes the main app shell
- [ ] `accounts.html` — Critical for understanding multi-account UX
- [ ] `scheduler.html` — Core value proposition; content calendar view
- [ ] `composer.html` — Post creation studio with multi-platform preview

### Medium Priority (Features)
- [ ] `analytics.html` — Charts, graphs, follower growth timeline
- [ ] `inbox.html` — Unified social inbox with filtering
- [ ] `reports.html` — Report builder

### Lower Priority (Marketing & Auth)
- [ ] `pricing.html` — Pricing page
- [ ] `login.html` — Login / sign up
- [ ] `onboarding.html` — New user flow
- [ ] `settings.html` — Settings and integrations

---

## 6. Creative Freedom Guidelines
*When the backlog is empty, follow these guidelines.*

1. **Stay On-Brand:** Every page must feel like it belongs in a premium dark SaaS product
2. **Enhance the Core:** Pages should support social media management workflows
3. **Naming Convention:** Lowercase, hyphenated filenames (e.g., `team-members.html`)

### Ideas to Explore
*Pick one, build it, then REMOVE it from this list.*

- [ ] `team.html` — Team workspace: member roles, permissions, activity log
- [ ] `integrations.html` — Third-party integrations marketplace (Zapier, Slack, Canva, etc.)
- [ ] `ai-assistant.html` — AI caption writer and hashtag suggester interface
- [ ] `brand-kit.html` — Brand kit manager: logos, color palettes, fonts, approved assets
- [ ] `notifications.html` — Notifications center: alerts, mentions, scheduled reminders

---

## 7. Rules of Engagement
1. Never recreate pages already marked `[x]` in Section 4
2. Always update `.stitch/next-prompt.md` before completing an iteration
3. Always include the full **DESIGN SYSTEM block** from `.stitch/DESIGN.md` Section 6 in every baton
4. Consume ideas from Section 6 after using them — remove the item
5. After generating a screen, update `.stitch/metadata.json` with the new screen's ID and metadata
