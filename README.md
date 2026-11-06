# MediCentrix Desktop — Prototype

A static, installable Progressive Web App (PWA) medication-list organizer. No backend, login, or Azure connection. Uses localStorage, which is **not encrypted and not suitable for confidential patient records**.

## Running locally

From the folder, run `python3 -m http.server 8000` and open `http://localhost:8000` (localhost is eligible for PWA testing). The site must be served from a web server, not opened using `file://`.

## Deploy

Push these files to a GitHub repository and import into Vercel as an **Other** project with no build command. Keep Vercel's temporary domain until testing is complete. Vercel provides HTTPS, which is required for PWA service workers.

## Windows installation

Open the deployed URL in Microsoft Edge or Chrome; use the browser's **Install app** option. If the browser emits a `beforeinstallprompt` event, the header also shows an install button. Browser installation UX varies; it is not a direct `.exe` download.

## Notes

- This is a functional prototype, **not** the contractors' clinical platform.
- Do not enter identifiable patient information; other users sharing the browser profile may be able to see data.
- Storage is browser-local and can be erased when site data is cleared.
- Exported CSV is unencrypted; protect it appropriately.
- No medication interaction checking, medical advice, medication alerts, or cloud syncing.
- The USPTO/attorney must determine whether actual use, the distribution mechanism, specimen, and claimed goods satisfy Class 9.
