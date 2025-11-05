# Ascendify

An AI-powered study companion for A-level (and later IB) students. This repo is optimised for employers and collaborators to quickly understand the product vision, technical direction, and how to contribute.

<p align="center">
  <img alt="Ascendify banner" src="docs/banner.png" width="780"/>
</p>

## TL;DR

- Mission: Personalised study plans, daily sessions, and adaptive question rewording to raise grades with less grind.
- Status: MVP in active build; this repo tracks the architecture, roadmap, and issues.
- For reviewers: Start with [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md), then skim [ROADMAP.md](ROADMAP.md) and open Issues.

## Key Features (MVP scope)
- AI Study Plan Generator (syllabus-aware, confidence-weighted)
- Daily Session Builder (timeboxed, spaced-repetition aware)
- AI-Enhanced Question Reworder (scaffolds from simple -> exam-style)
- Progress Dashboard (mastery, weak-topic surfacing, streaks)

## Tech Direction
This repo is tech-agnostic by design for now. Initial target stack (subject to change as the MVP evolves):
- Web App: Next.js (TypeScript), Tailwind
- API: FastAPI (Python) or Next.js API routes
- DB: PostgreSQL (Prisma/SQLModel)
- Auth: Clerk/Auth.js
- AI: OpenAI-compatible LLMs; RAG for syllabus-aligned retrieval
- Infra: Vercel (web), Fly.io/Render (API), Supabase/Neon (DB)

If you are an employer: this split demonstrates architectural judgment; details will track in Issues and PRs.

## Quick Start (Docs-first)
```bash
# 1) Fork or clone
git clone https://github.com/YOUR-USER/ascendify.git
cd ascendify

# 2) Explore docs
open docs/ARCHITECTURE.md  # or code docs/*
open ROADMAP.md

# 3) Pick an issue
# See labels: good-first-issue, help-wanted, design, backend, frontend
```

## Repository Map
```
.
├─ docs/                 # design docs, diagrams, decisions
├─ .github/
│  ├─ ISSUE_TEMPLATE/    # bug + feature templates
│  └─ workflows/         # CI stubs
├─ ROADMAP.md
├─ CHANGELOG.md
├─ SECURITY.md
├─ CODE_OF_CONDUCT.md
├─ CONTRIBUTING.md
└─ LICENSE
```

## Badges
![CI](https://img.shields.io/badge/CI-ready-lightgrey)
![License: MIT](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/status-MVP--in--progress-blue)

## Demo & Media
- Short Loom/TikTok demo planned — placeholder here.  
- Marketing one-pager lives in `docs/one-pager.md` (optional).

## Contact
- Maintainer: Muhammed Ismaeel Naveed (Ismaeel) — open to SWE internships and B2B collaborations.
- Email: add later | LinkedIn: add later
