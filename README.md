# 2028 Nomination Draft

Live snake drafts for the 2028 Democratic and Republican presidential nominations.
Picks sync in real time for everyone with the link through Firebase Firestore, and the
site is hosted on GitHub Pages.

## Files

- `index.html` – the whole site
- `firebase-config.js` – the Firebase web app settings (public identifiers, not secrets)
- `firestore.rules` – database rules to paste into Firebase console > Firestore > Rules
- `seed.json` – starting players, settings and candidate pool, loaded automatically the
  first time the site opens against an empty database

## Setup

1. Create a Firebase project, add a Cloud Firestore database (production mode), and paste
   `firestore.rules` into its Rules tab.
2. Register a web app in Project settings and copy its `firebaseConfig` values into
   `firebase-config.js`.
3. Turn on GitHub Pages: Settings > Pages > Deploy from a branch > `main` / root.
