# Bus Count

A private, offline-capable web app (PWA) for recording twice-daily bus rider counts on an iPhone.

- Fields: date, start time, stop time, Cole count, Spofford count (total is calculated)
- Data is stored only on the device (localStorage); nothing is sent anywhere
- Fridays after noon, a banner reminds you to export a backup CSV (hidden once you have exported that day)
- Export to CSV, or build a printable report for a date range (Print / Save as PDF)

## Install on iPhone (no Mac needed)

1. Host this folder over HTTPS (GitHub Pages, Netlify, Cloudflare Pages, etc.)
2. Open the URL in Safari, tap Share, then Add to Home Screen

## Updating

After changing any file, bump `CACHE` in `sw.js` (currently `buscount-v6`) so installed copies refresh.

## Files

- `index.html` – the whole app (HTML, CSS, JS)
- `manifest.json`, `icon-*.png` – home screen install metadata
- `sw.js` – service worker for offline use
