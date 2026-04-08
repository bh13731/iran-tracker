# Iran Missile & Drone Tracker

Live depletion tracker for the 2026 Iran conflict. Tracks ballistic missiles, cruise missiles, drones, and launcher attrition across all theaters using official Gulf state intercept data, IDF reporting, and ISW/CTP assessments.

**Live site:** [bh13731.github.io/iran-tracker](https://bh13731.github.io/iran-tracker/)

## What this tracks

- **UAE MoD cumulative intercepts** (highest-confidence series)
- **Total munitions fired** across all theaters (confirmed floor + best-estimate range)
- **Launcher depletion** — the binding constraint on Iran's BM capability
- **Gulf breakdown by country** — stacked intercepts across UAE, Kuwait, Qatar, Bahrain, Saudi Arabia, Israel
- **Stockpile snapshot** — pre-war estimates vs. fired vs. remaining, with confidence ratings

## Repository structure

```
index.html          — Main dashboard (D3.js, no build step)
data.json           — Normalized dataset powering the charts
methodology.html    — How the tracker works, source hierarchy, caveats
stories/            — Data-driven analysis pieces
  index.html        — Stories listing
  2026-04-08-*.html — First story: cease-fire analysis
source/             — Raw analytical source files
  current-state.md  — Latest tracker summary
  ledger.md         — Structured cumulative reference (every official data point)
  daily-log.md      — Dated daily analytical notes
  methodology.md    — Methodology in plain Markdown
  archive/          — Pre-restructure historical tracker (Days 1-20)
```

## Data sources

- UAE MoD official cumulative intercept counts
- Bahrain Defence Force official reporting
- IDF launcher attrition / strike reporting
- ISW / CTP Special Reports
- Saudi MoD, Kuwait MoD, Qatar MoD (working estimates)
- Wikipedia conflict article cross-references

See [methodology.html](methodology.html) for the full source hierarchy and caveats.

## Serve locally

```bash
# Any static file server works:
python3 -m http.server 8080
# or
npx serve .
```

## License

Data is compiled from public sources. Analysis is original. Use with attribution.
