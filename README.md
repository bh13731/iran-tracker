# Iran Missile & Drone Tracker — Static Site

Interactive D3.js visualization of Iran's missile/drone depletion during the 2026 conflict.

## Serve locally

```bash
# Any static file server works:
cd iran-tracker-site
python3 -m http.server 8080
# or
npx serve .
```

Then open `http://localhost:8080`.

## Files

- `index.html` — Single-page app (D3 via CDN, no build step)
- `data.json` — Normalized dataset extracted from the tracker source files

## Data sources

- UAE MoD official cumulative intercept counts (highest confidence)
- ISW/CTP Special Reports
- Bahrain Defence Force, Kuwait MoD, Saudi MoD, Qatar MoD
- IDF launcher attrition reporting
- Wikipedia conflict article cross-references
