# Canucks Ticket Ledger — GitHub Pages deploy

## What's in here
- `docs/index.html` — your private owner dashboard (sign-in required)
- `docs/listing.html` — the public customer-facing listing page (no sign-in)
- `firestore.rules` — reference copy of the security rules already published in the Firebase console (not used by GitHub Pages, just kept here for reference)
- `firebase.json` — not needed for GitHub Pages, only relevant if you ever switch to Firebase Hosting later

## Deploy steps (no terminal needed)
1. Upload this whole folder to a GitHub repo (drag the folder into "Add file → Upload files").
2. In the repo: **Settings → Pages** → Source: "Deploy from a branch" → Branch: `main`, folder: `/docs` → Save.
3. Wait ~1 minute, then your site is live at:
   `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`
4. In the Firebase console: **Authentication → Settings → Authorized domains** → Add `YOUR_USERNAME.github.io`.
5. Visit `.../index.html`, sign in, confirm your 42 games load.
6. Visit `.../listing.html` to see the public page.

Both HTML files already have your live Firebase config and security rules baked in — nothing else to edit.
