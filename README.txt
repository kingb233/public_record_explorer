PUBLIC RECORD EXPLORER — OFFLINE-FIRST PWA

Files:
- index.html: app shell
- app.js: search/navigation/record viewer
- style.css: mobile interface
- records.json: local database exported from the Excel master
- manifest.webmanifest: install metadata
- sw.js: offline cache

IMPORTANT:
A PWA must be served over HTTPS (or localhost) for installation/service-worker offline caching.
Opening index.html directly from an iPhone file preview will not provide the full app runtime.

Once installed from an HTTPS host:
- all included records/search/category browsing work offline;
- external source hyperlinks require internet only when opened;
- updating records.json and the service-worker cache version publishes a database update.

The Excel workbook remains the research/master database. records.json is the app-readable export.
