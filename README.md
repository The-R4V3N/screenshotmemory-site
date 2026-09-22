# ScreenshotMemory Site

This repository contains the official public product website for ScreenshotMemory.

ScreenshotMemory is an Android-first app that discovers screenshots, understands their contents locally, and resurfaces them when they may be useful.

## Live site

- [Product site](https://the-r4v3n.github.io/screenshotmemory-site/)
- [Privacy Policy](https://the-r4v3n.github.io/screenshotmemory-site/privacy/)
- [Support](https://the-r4v3n.github.io/screenshotmemory-site/support/)

## About ScreenshotMemory

ScreenshotMemory is a focused screenshot organization and resurfacing utility rather than a generic gallery. Its core loop is:

Screenshot → Discover → Understand → Remember → Resurface → Act / Later / Forget

The product is local-first: OCR and classification run on-device, no ScreenshotMemory account is required, and ScreenshotMemory does not provide cloud synchronization, advertising, or analytics/tracking.

## Site architecture

The website deliberately uses:

- Plain HTML and plain CSS
- No framework or build system
- No JavaScript requirement
- No analytics/tracking or cookies
- No backend
- No external fonts or scripts

The simplicity is intentional: GitHub Pages can serve the site directly with minimal maintenance.

## Repository structure

```text
.
├── index.html
├── privacy/
│   └── index.html
├── support/
│   └── index.html
├── assets/
│   ├── icon.png
│   ├── favicon.png
│   ├── apple-touch-icon.png
│   └── screenshots/
├── styles.css
├── LICENSE
└── README.md
```

## Local preview

Serve the repository with Python's built-in static-file server:

```powershell
python -m http.server 8000
```

Then visit [http://localhost:8000/](http://localhost:8000/).

## Deployment

The site is deployed through GitHub Pages from the `master` branch at the repository root. No build step is required.

## Support

For privacy questions or product support, contact [r4v3n.development@gmail.com](mailto:r4v3n.development@gmail.com).
