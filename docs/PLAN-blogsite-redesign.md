# Plan: Redesign & Migration to Personal Academic Blog

## Objective
Transform `isratnipa28.github.io` into a high-grade, Substack-inspired academic & personal blog for **Israt Jahan Nipa**, drawing structural and aesthetic inspiration from `sai21112000.github.io` while reflecting Nipa's background as an AI Researcher and Educator.

---

## 🏗️ Architecture & Component Design

### 1. Site Branding & Header Navigation
- **Brand Logo / Initials**: `IJN` / `Nipa` logo badge with sleek font styling.
- **Primary Navigation**:
  - `Essays` (Writing & research notes)
  - `Publications` (Academic research papers, conference posters, preprints)
  - `Teaching` (Course notes, student resources)
  - `Philosophy` (Thoughts on AI ethics, education, and gentle technology)
  - `About` (Full bio, education, background, contact)
- **Header Actions**:
  - Theme Toggle (`◐` / `◑` dark and light mode)
  - Action Button (`Get in touch` or `Google Scholar`)

### 2. Homepage (`_layouts/home.html`)
- **Hero Intro Section**:
  - Avatar / Profile Portrait with circular glow / subtle shadow
  - Eyebrow: `AI Researcher · Senior Lecturer · Storyteller`
  - Headline: `Exploring AI, Federated Learning, and Human-Centric Technology`
  - Bio blurb detailing research interests and academic journey
- **Editorial Post Grid**:
  - Left column: Latest essays with reading time, publication date, tags, and category fallback media badges.
  - Right sidebar: Trending stories, featured publications, quick links (Google Scholar, ResearchGate, LinkedIn, GitHub).

### 3. Content Pages
- `writing.md`: Filterable archive of essays by category (`Research`, `AI`, `Tech`, `Life`).
- `about.md`: Structured academic profile, background, education, and contact form/link.
- `philosophy.md`: Essays on teaching philosophy and technological ethics.
- `publications.md` *(New)*: Organized list of research papers with links, abstracts, and PDF downloads.

---

## 📋 Task Breakdown

| Phase | Description | Files Modified/Created | Status |
|-------|-------------|------------------------|--------|
| **Phase 1** | Base Design System & CSS Optimization | `assets/style.css`, `_config.yml` | Pending |
| **Phase 2** | Layout Overhaul (Header, Hero & Footer) | `_layouts/default.html`, `_layouts/home.html` | Pending |
| **Phase 3** | Content & Page Integration | `about.md`, `writing.md`, `philosophy.md`, `publications.md` | Pending |
| **Phase 4** | Interactive Features (Theme Toggle, Lightbox, Progress Bar) | `_layouts/default.html`, `assets/style.css` | Pending |
| **Phase 5** | SEO & Metadata Audit | `_config.yml`, `feed.xml` | Pending |

---

## 🔍 Verification Checklist

- [ ] Page builds cleanly with Jekyll / GitHub Pages syntax.
- [ ] Theme toggle seamlessly switches light/dark modes without flash.
- [ ] Responsive navigation works smoothly across mobile and desktop viewports.
- [ ] All typography renders crisply (Inter & Source Serif 4 fonts).
- [ ] Google Scholar / GitHub links properly configured.
