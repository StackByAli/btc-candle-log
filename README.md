# BTC Candle Log — iPhone PWA starter

A mobile-friendly installable web app for recording one active bot per BTC 5-minute candle.

## Features
- Bot eligibility is based on previous candle colour and starting-price group.
- Exactly one active bot per candle.
- Records are saved immediately in IndexedDB in the browser on this iPhone.
- Each record keeps the date selected in the candle timestamp (`candleDate`).
- Select a date in **Choose day to export** and download only that day's CSV, for example `btc-candle-records-2026-10-23.csv` and `btc-candle-records-2026-10-24.csv`.
- CSV files open in Excel or Apple Numbers.

## Important storage note
Local means stored in this Safari/PWA browser on this device, not synced live to a cloud server or MySQL. Keep a regular export backup. Do not clear Safari website data if you need records that have not been exported. If you remove/reinstall the website app or browser storage is cleared, records may be lost.

## Deploy using GitHub Pages
Upload `index.html`, `manifest.json`, and `sw.js` to a GitHub repository, enable Settings → Pages for the `main` branch and root folder, then open the published HTTPS address in Safari on iPhone and choose Share → Add to Home Screen.

This is a PWA, not a native App Store app. It has no automatic cloud backup and no MySQL integration.
