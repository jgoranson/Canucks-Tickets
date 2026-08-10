# Canucks Ticket Ledger — GitHub Pages deploy

## What's in here
- `docs/index.html` — your private owner dashboard (sign-in required)
- `docs/listing.html` — the public customer-facing listing page (no sign-in)
- `firestore.rules` — reference copy of the security rules already published in the Firebase console
- `firebase.json` — not needed for GitHub Pages, only relevant if you switch to Firebase Hosting later

## Deploy steps (no terminal needed)
1. Upload the contents of this folder to your GitHub repo (drag `docs` and `README.md` in via "Add file → Upload files").
2. In the repo: Settings → Pages → Source: "Deploy from a branch" → Branch `main`, folder `/docs` → Save.
3. Site goes live at: https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/
4. Firebase console → Authentication → Settings → Authorized domains → add `YOUR_USERNAME.github.io`.
5. Visit `.../index.html`, sign in, confirm all 44 games load (42 regular season + 2 preseason).
6. Visit `.../listing.html` to see the public page — merged seat pairs, team badges, past games hidden.
