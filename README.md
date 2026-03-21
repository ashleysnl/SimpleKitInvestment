# SimpleKit Compound Interest Calculator

This repository contains a static compound interest calculator built on the shared SimpleKit shell.

The tool helps users estimate:

- how an initial investment may grow over time
- how recurring contributions affect compound growth
- how compounding changes long-term investment outcomes
- how fees and inflation can reduce the ending value
- the difference between contributions and investment gains

## What It Includes

- static HTML, CSS, and JavaScript only
- shared SimpleKit core shell, navigation, and footer
- preserved Google Analytics head snippet
- compound interest and investment growth simulation with:
  - monthly, biweekly, or annual contributions
  - annual, semi-annual, quarterly, or monthly compounding
  - optional fee drag
  - optional inflation adjustment
  - optional annual contribution increases
  - optional future lump-sum contribution
- native SVG charts
- year-by-year projection table
- CSV export for the detailed table
- SEO metadata and FAQ structured data
- educational content for compound interest, contributions, fees, and inflation
- related-tool links across the SimpleKit planning ecosystem

## Run Locally

Because this is a static site, you can open `index.html` directly in a browser or serve the folder with a simple local server.

Example:

```bash
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/
```

## File Structure

```text
/
  index.html
  assets/
    css/
      styles.css
    js/
      app.js
  README.md
```

## Implementation Notes

- The shared SimpleKit shell is still loaded from `https://core.simplekit.app`.
- The Google Analytics snippet in `index.html` was preserved.
- The calculator uses a fine-grained client-side simulation so contribution timing, compounding cadence, fee drag, and yearly rollups stay consistent.
- Charts are rendered with lightweight inline SVG instead of a chart library to keep the app static and dependency-free.
- The app is branded around `Compound Interest Calculator` with the supporting subtitle `Investment Growth With Contributions` to better match high-intent search behavior while preserving the existing calculation engine.
- No route or slug change was made in this pass so existing deployments and links stay stable.
