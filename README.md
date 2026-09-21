# ScreenshotMemory website

The official static public website for ScreenshotMemory. It provides a small product landing page plus the public Privacy Policy and Support URLs needed for the Google Play release.

This repository is intentionally plain HTML and CSS. There is no build system, package manager, analytics, cookies, or backend service.

## Structure

- `index.html` — product landing page
- `privacy/index.html` — canonical Privacy Policy path (`/privacy/`)
- `support/index.html` — public Support path (`/support/`)
- `styles.css` — shared responsive, light/dark-mode styles
- `assets/` — approved product assets when they become available

## GitHub Pages

After merging the desired branch into `master`, configure GitHub Pages to deploy from the `master` branch and the repository root (`/`). GitHub Pages will then serve the site without a build step.

For a project site at `https://&lt;username&gt;.github.io/ScreenshotMemory-Site/`, the canonical policy URL is:

`https://&lt;username&gt;.github.io/ScreenshotMemory-Site/privacy/`

All site links are relative, so they work under that repository path rather than requiring a domain-root deployment.

## Local preview

Open `index.html` in a browser for a basic preview. To test directory URLs and navigation more closely, serve the repository with any local static-file server, for example from PowerShell:

```powershell
python -m http.server 8000
```

Then visit `http://localhost:8000/`. No dependency installation is required.

## Content maintenance

Add only official, approved product assets when they are available.
