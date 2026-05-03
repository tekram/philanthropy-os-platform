# Changelog

All notable changes to Philanthropy OS are documented here.

---

## [2026-05-03] Charity Data Enrichment + Live Campaigns + Lead Pipeline

### Added
- **83 real charities** with verified EINs, websites, accurate missions, and standardized cause tags (was 104 with fake data)
- **Live Campaigns** — 113 real campaigns seeded across 80 directory orgs, displayed in Transparency Layer with "Donate on their site →" external links
- **Lead Pipeline Dashboard** — admin view ranking unregistered orgs by weighted donor engagement (views×1 + clicks×3 + favorites×5 + AI recs×2) for outreach prioritization
- **Engagement tracking** — page views, campaign clicks, and favorites tracked per unregistered org in Firestore
- **External donate flow** — directory orgs route to their real donation pages; registered orgs (OBAT, TCF-USA) keep in-platform flow
- `website` and `isRegistered` fields on `Nonprofit` type
- `LiveCampaign` type for campaign data from directory orgs
- `website` field included in Gemini AI prompt context for smarter recommendations
- Firestore seed scripts: `seed-nonprofits.ts` (org metadata) and `seed-live-campaigns.ts` (campaign data)

### Changed
- **Tag vocabulary standardized** — dropped vague tags (`Arts & Culture`, `Poverty Alleviation`, `Global Reach`, `Empowerment`); replaced with actionable taxonomy: cause areas, focus populations, approach, geography
- **Nonprofit array cleaned** — removed 21 non-donatable entities (foundations, government agencies, testing bodies)

### Architecture
- Engagement counters use Firestore `increment()` — best-effort, silent on failure
- Live campaigns stored at `nonprofits/{id}.liveCampaigns` with `liveCampaignsUpdatedAt` timestamp
- Lead Pipeline reads engagement data from Firestore and computes weighted scores client-side

### Deferred (Phase 4)
- Scheduled Cloud Function for nightly campaign refresh
- Gemini grounding endpoint for on-demand live campaign fetching
- Stale campaign badge (>48h)
- Per-org admin force-refresh button