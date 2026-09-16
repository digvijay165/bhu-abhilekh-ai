# Bhu-Abhilekh AI

**AI-Powered Digitisation of Legacy Land Records** — a Smart India Hackathon 2026 prototype.

AI converts old handwritten land records (across 20+ Indian scripts) into searchable,
verified, GIS-linked digital records — cutting the time to retrieve a certified copy
from two weeks to two minutes.

## What's in this repo

A single-page React website (`index.html`) that demonstrates the product concept:

- Hero section with the pitch and key stats
- Problem / solution overview
- **Interactive live demo** — search a mock dataset of digitised land records by name,
  village, or khasra/survey number, with language filters and a record detail view
  (scanned document placeholder, extracted fields, verification badge, GIS map pin)
- Six-stage technical pipeline (Scan → Pre-processing → OCR+HTR → Layout & NER →
  Human Verify → Search & GIS) with the full tech stack
- Citizen journey (today vs. with the platform), impact stats, feasibility, and
  a three-phase roadmap

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
