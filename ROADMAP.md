# Philanthropy OS — Product Roadmap

A persistent "Giving Layer" that follows donors across the web — replacing fragmented donation experiences with a portable, AI-powered **Impact Passport**.

Legend: ✅ Complete · 🔄 In Progress · 🔲 Planned

---

## Phase 1 — Donor Core

| Feature | Status |
|---|---|
| Conversational donor onboarding (values, interests, budget, giving style) | ✅ Complete |
| Impact Passport — portable philanthropic identity card with QR code | ✅ Complete |
| Values Discovery Assistant — 4-question AI extraction engine | ✅ Complete |
| Donor profile (causes, giving mode, monthly budget, employer match) | ✅ Complete |
| Account role selector (donor ↔ NGO dual-account) | ✅ Complete |
| Giving History & ledger (IRS-compliant, immutable) | ✅ Complete |
| Donor settings panel (budget, mode, interests, employer match) | ✅ Complete |

---

## Phase 2 — Transparency & Trust Index

| Feature | Status |
|---|---|
| Charity Index / Transparency Layer (50+ curated nonprofits + IRS database) | ✅ Complete |
| Trust Index scores from IRS 990 data (efficiency, overhead, CEO pay) | ✅ Complete |
| Filter by cause area (Climate, Education, Health, etc.) | ✅ Complete |
| Curated vs global search toggle | ✅ Complete |
| Platform Partner badge for onboarded NGOs | ✅ Complete |
| Campaign Discovery — Gemini-powered live search for nonprofit initiatives | ✅ Complete |
| Charity Navigator API integration (225k+ orgs) | 🔲 Planned |
| Candid / GuideStar API integration | 🔲 Planned |
| GreatNonprofits community reviews layer | 🔲 Planned |
| Nonprofit Health Alerts (rating drops, leadership changes) | 🔲 Planned |

---

## Phase 3 — Agentic Giving Engine

| Feature | Status |
|---|---|
| Manual giving mode — direct charity selection & amounts | ✅ Complete |
| Copilot mode — AI-suggested plan with donor approval | ✅ Complete |
| Autopilot mode — fully automated allocations from profile | ✅ Complete |
| Giving Strategy Planner — chat-driven plan refinement | ✅ Complete |
| Employer match surfacing (database, eligibility check, effective gift calc) | ✅ Complete |
| HR portal deep-links for match claiming | ✅ Complete |
| Tax Optimization Engine (bunching strategies, year-end alerts, IRS receipts) | 🔲 Planned |
| Micro-Giving Roundup (Plaid bank roundup → agentic distribution) | 🔲 Planned |

---

## Phase 4 — Crisis Pulse Engine

| Feature | Status |
|---|---|
| Real-time crisis feed (earthquake, flood, conflict, epidemic, etc.) | ✅ Complete |
| Severity levels 1–5 with geolocation mapping (Leaflet) | ✅ Complete |
| Crisis Responder Badge — flags orgs actively responding | ✅ Complete |
| Crisis alignment filtering (show crises matching donor values) | ✅ Complete |
| Crisis notification strip (sticky header with active alerts) | ✅ Complete |
| Crisis Responder Mode — auto-redirect 5–50% of budget to crisis orgs | ✅ Complete |
| Multi-source crisis ingestion (USGS, GDACS, ACLED, UNHCR, WHO, FEMA) | 🔲 Planned |
| 2-source confirmation before alerting (anti-false-alarm layer) | 🔲 Planned |
| Human review layer for contested classifications | 🔲 Planned |

---

## Phase 5 — Embeddable Widget & NGO Tools

| Feature | Status |
|---|---|
| Embeddable concierge widget (iframe, transparent bg, auto-resize) | ✅ Complete |
| In-widget donation modal with guest checkout | ✅ Complete |
| Magic link / Passport claim for guest donors post-signup | ✅ Complete |
| Intent-triggered Passport CTAs inside widget | ✅ Complete |
| NGO onboarding & portal (profile, EIN, mission, donors, projects) | ✅ Complete |
| Active Donor Network — value-alignment matching for NGOs | ✅ Complete |
| Admin control center — approve/deny NGO applications | ✅ Complete |
| Nonprofit data pipeline (B2B API for private donor + impact data sync) | 🔲 Planned |
| Automated impact feedback (show specific outcomes of prior donations) | 🔲 Planned |
| Predictive project resonance modeling per visiting donor | 🔲 Planned |

---

## Phase 6 — AI Concierge

| Feature | Status |
|---|---|
| Floating Concierge Agent — context-aware chat on all donor pages | ✅ Complete |
| Three-voice message system (agent, platform, nonprofit) | ✅ Complete |
| Alignment percentage chips and follow-up suggestion chips | ✅ Complete |
| Crisis context injection (live responder info in chat) | ✅ Complete |
| Trust score and 990 data surfaced in chat | ✅ Complete |
| Employer match explanation and suggestions in chat | ✅ Complete |
| Onboarding chat (structured extraction via Gemini Flash) | ✅ Complete |
| Planning chat (strategy refinement, allocation recalculation) | ✅ Complete |
| AI Impact Storytelling Engine (personalized shareable impact narratives) | 🔲 Planned |

---

## Phase 7 — Community & Legacy

| Feature | Status |
|---|---|
| Year in Giving Report (annual impact report with visualizations) | 🔲 Planned |
| Value Evolution Tracking (giving pattern shifts + portfolio rebalancing) | 🔲 Planned |
| Giving Circles (family/workplace groups, Circle Passport, voting on allocations) | 🔲 Planned |
| Legacy & Estate Layer (DAFs, charitable trusts, bequest giving) | 🔲 Planned |

---

## Public-Facing Pages

| Feature | Status |
|---|---|
| Landing page with transparency index CTA | ✅ Complete |
| Public Transparency Index (unauthenticated charity search) | ✅ Complete |
| Charity Partners page | ✅ Complete |
| Charity Landing Page / Demo mode with live concierge | ✅ Complete |

---

## Tech Stack

- **Frontend:** React + Vite + Tailwind v4 + Framer Motion
- **Backend:** Express + Firebase Firestore + Firebase Auth
- **AI:** Google Gemini Flash (conversational discovery, RAG, strategic planning, campaign search)
- **Design:** Fraunces (serif) + Inter (sans) + JetBrains Mono; two-tone donor/admin token system

---

## Grant & Partnership Context

- Grant target: Bill & Melinda Gates Foundation Grand Challenge on AI for Charitable Giving
- Pilot partner: OBAT Helpers Inc. (fiscal sponsor, first integration site)
- OBAT committed to recruiting 3 additional charities within 6 months of launch
