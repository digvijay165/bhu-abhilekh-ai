# Terra Trust

**AI-Verified Land Records & Citizen Services** — a Smart India Hackathon 2026 prototype.

A full citizen-services portal (in the style of state land-record portals) built on top
of an AI pipeline that converts old handwritten land records — across 20+ Indian scripts —
into searchable, verified, GIS-linked digital records. Cuts the time to retrieve a
certified copy from two weeks to two minutes.

## What's in this repo

A single-page React app (`index.html`) with six tab-based sections:

- **Home** — hero, a live cadastral parcel highlight card, an instant application
  tracker, a services preview, a citizen knowledge hub, and a compliance disclaimer
- **Services** — the full grid of citizen services (registration, mutation, records
  search, title check, duty calculator, dispute & zoning)
- **Land Records** — search a mock dataset of digitised records by name, village, or
  khasra/survey number, with language filters, a scanned-document preview, extracted
  fields, a GIS map pin, and linked documents
- **Applications** — search and track mutation/registration dockets with a live
  4-stage progress tracker, assigned authority, and dates
- **Documents** — every document linked to a citizen's verified records, with
  verification status
- **Platform** — the AI pipeline (Scan → Pre-processing → OCR+HTR → Layout & NER →
  Human Verify → Search & GIS), full tech stack, impact stats, and roadmap, for
  hackathon reviewers

Other touches: a working **EN/हिंदी language toggle**, a notifications dropdown, a
profile menu, and a mobile app-style bottom nav with a "More" sheet.

## Tech

Built with **React 18** and **JavaScript**, loaded via CDN with Babel standalone —
no build step required. Just open `index.html`, or serve it with any static file server:

```bash
python -m http.server 8080
# then open http://localhost:8080
```

## Status

Front-end prototype with mock data, built for the SIH 2026 pitch. The production
pipeline (OCR/HTR, LayoutLMv3, PostGIS, Elasticsearch, etc.) is described in the
Technical Approach section but not implemented here.
