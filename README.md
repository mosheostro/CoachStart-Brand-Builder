# Coach Start

Self-contained, single-file React+Babel landing page for the Coach Start brand-builder product.

## Structure

```
Claude/Coach-Start/
├── index.html        # Main page (React + Babel via CDN, in-browser compile)
├── coach-start.html  # Identical copy under the original filename
└── README.md
```

## Run locally

The file has no build step. Any static HTTP server works:

```bash
# Python 3
cd /c/Users/evgen/Claude/Coach-Start
python -m http.server 4321

# Then open: http://localhost:4321
```

Or open `index.html` directly in a browser — Chrome/Edge/Firefox/Safari all work.

## Dependencies

All loaded from CDNs at runtime — no `node_modules`, no package manager:

- `react@18.3.1` (unpkg)
- `react-dom@18.3.1` (unpkg)
- `@babel/standalone@7.29.0` (unpkg)
- DM Serif Display + DM Sans (Google Fonts)

## Languages

EN / RU / HE (RTL) / DE — switchable via the language picker in the nav. Theme toggle for light/dark.

## Origin

This project was extracted from the `wefi-portal-next` worktree (`public/coach-start.html`). It is now fully isolated — no WeFi code, no shared imports.
