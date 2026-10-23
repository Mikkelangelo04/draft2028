# 2028 Nomination Draft

Live snake drafts for the 2028 Democratic and Republican presidential nominations.
Picks sync in real time through Firebase Firestore, and the site is hosted on GitHub Pages.
A landing page asks for the league password, which signs the visitor in to one shared
Firebase account; the database rules only serve data to that account.

## Files

- `index.html` – the whole site
- `firebase-config.js` – the Firebase web app settings (public identifiers, not secrets)
- `firestore.rules` – database rules to paste into Firebase console > Firestore > Rules

## Setup

1. Create a Firebase project, add a Cloud Firestore database (production mode), and paste
   `firestore.rules` into its Rules tab.
2. Register a web app in Project settings and copy its `firebaseConfig` values into
   `firebase-config.js`.
3. In Authentication > Sign-in method, enable Email/Password, then add the user
   `players@draft2028-e569a.firebaseapp.com` with the league password.
4. Turn on GitHub Pages: Settings > Pages > Deploy from a branch > `main` / root.
