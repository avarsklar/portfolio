---
type: reference
tags: [portfolio, pm-layer]
---

# PM Layer — Portfolio

*Last updated: 2026-07-07*

### 1. What & Why
A one-page personal portfolio site that presents Ava as an AI-native product builder and PM to recruiters, collaborators, and anyone she's sending her work to. It exists so she can drop a single link — `avarsklar.github.io/portfolio` — and have her story, work, and contact info land instantly, looking like someone who ships things with taste.

### 2. Definition of Done
The site is already live and showing real work. "Done" here means the page a recruiter lands on is accurate and trust-building:

- [x] Bold redesign live — custom typography (Bricolage Grotesque + Fraunces + Space Mono), sand/vermilion palette, grain texture, scroll-reveal animations (`index.html` — commit `858206c`)
- [x] Flagship project (Refit) presented with a screenshot carousel and live link to `bucknellrefit.com` (`index.html` — carousel confirmed in source)
- [x] All sections populated: hero, education band, work grid (Refit, Lead Developer, Club Ralley, restaurant analytics, accessible games), skills chips, research section (infant eye movement, burnout paper, SUDEP), contact (`index.html`)
- [x] Accessibility baseline present: skip link, `aria-live` for carousel, focus-visible styles, `prefers-reduced-motion` support, minimum 44px touch targets on nav links (`index.html`)
- [x] GitHub Pages deploy wired from `main` via `.github/workflows/pages.yml` — push = live in ~1 min (`CLAUDE.md`)
- [x] Traction figure displayed on the flagship card (`index.html`) — ⚠️ currently reads "~150 active users," which overstates it (see fix below)
- [ ] **Fix the live traction copy** — real numbers are ~150 users total, ~20 active (sold / liked / purchased) (Ava, 2026-07-07). The card's "~150 active users" overstates it; change to "~150 users · ~20 active" — honest and still a real receipt — before any recruiter share
- [ ] Contact email: uses `ars038@bucknell.edu` — confirm whether a personal address should replace this before the site goes to a recruiter outside Bucknell

> TODO (couldn't confirm from repo): Whether a Workboard / dedicated now-next list for Portfolio exists anywhere — `CLAUDE.md` says "No dedicated workboard file; check `~/ava-os/📋 Projects.md` (Portfolio row)." The Projects.md row reads "shipped · idle backlog only · 2026-07-02."

### 3. Roadmap — Now / Next / Later

- **Now** — None. The site is shipped and in idle-backlog mode (Projects.md, row last updated 2026-07-02). No active sprint.
- **Next** — Refresh case studies when new work ships: update the Refit traction number as Bucknell Refit grows; add Club Ralley once it has a launch moment worth featuring; add the Lead Developer skills site link once that ships. Each of these is a small text/asset edit — no structural change needed.
- **Later** — A full case-study expansion if the site ever needs to serve a longer hiring process (detailed project write-ups, outcomes, process narrative). The current one-pager is the right format for now; case studies only make sense when there's a reason to go deeper. Also: swap `ars038@bucknell.edu` for a permanent email before graduation (May 2028).

### 4. Milestones — Alpha / Beta / Release

| Stage | What it means for this site | Rough when |
|---|---|---|
| **Alpha** | Basic site live with name, role, and at least one project. | Reached (commit `c734030` — "Initial portfolio site") |
| **Beta** | Research, skills, and all major projects present; self-contained and shareable as a first impression. | Reached (commits `673eed9`–`8b18e7d` — restructure + research + games content added) |
| **Release** | Bold redesign live; Refit as flagship with screenshot carousel; accurate traction numbers; deployed on GitHub Pages with auto-deploy wired. | Reached 2026-07 (commits `858206c` + `b1cac9b` — redesign + carousel; Pages live at `avarsklar.github.io/portfolio`) |

### 5. Features / Sprints

No active sprint. The site is in idle-backlog mode.

The only "work in flight" is passive maintenance: keeping traction numbers and featured-project status current as the underlying projects evolve. No workboard file exists for this project — per `CLAUDE.md`, track any future work in `~/ava-os/📋 Projects.md` (Portfolio row) or in the git log.

**Stack (from `CLAUDE.md` + `index.html`):**
- Vanilla HTML + CSS + JavaScript — no framework, no npm, no build step (intentional; keep it that way)
- Hosted on GitHub Pages, auto-deployed from `main` via `.github/workflows/pages.yml`
- External fonts via Google Fonts (Bricolage Grotesque, Fraunces, Newsreader, Space Mono)
- Assets: `assets/` directory with headshot, game screenshots/videos, SUDEP PDF, and Refit app screenshots
