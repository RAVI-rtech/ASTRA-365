# ASTRA 365 — GitHub Pages PWA

A browser-first productivity workspace with a premium purple/blue interface.

## Included
- Home dashboard and app launcher
- ASTRA Docs: editable document surface, formatting toolbar, local save, print-to-PDF
- ASTRA Sheets: editable grid, CSV export, local save
- ASTRA Slides: editable slide canvas and print-to-PDF
- ASTRA PDF: text/image print-to-PDF workflow
- ASTRA Drive: upload/download/delete files and export workspace backup
- Notes, Calendar, Tasks, Forms, local demo Chat and drawing Board
- PWA manifest and offline service worker

## Deploy to GitHub Pages
1. Create a GitHub repository, for example `astra-365`.
2. Extract this ZIP and upload **all files inside** the folder to the repository root.
3. Open repository **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch `main`, folder `/ (root)`, then Save.
6. Wait for the deployment URL. Open it in Chrome.
7. On Android Chrome, use browser menu → **Install app** or **Add to Home screen**.

If deploying to a project subpath such as `https://username.github.io/astra-365/`, the relative paths in this project are already configured for that.

## Important limitations
This is a functional front-end starter, not a full Microsoft 365 replacement yet.
- Data is stored in browser localStorage; it does not sync across devices.
- Chat is a local demo, not real-time multi-user messaging.
- Docs/Slides are lightweight editors, not full DOCX/PPTX-compatible suites.
- Sheets supports cell editing and CSV export, not formulas or XLSX compatibility.
- PDF creation uses the browser print dialog. Choose **Save as PDF**. Advanced merge, split, compression, OCR and page editing are not implemented.
- Drive uploads are browser-local and storage is subject to browser quotas.
- For real accounts, cloud storage, collaboration and cross-device sync, add a secure backend such as Supabase in a later phase.

## Local testing
You can open `index.html` for basic testing. PWA installation and service worker offline caching require HTTPS or localhost.
