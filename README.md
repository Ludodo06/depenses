# Mes dépenses

Personal app to track my expenses, on my phone and on my computer.
One HTML page, no build step. Run locally with `python3 -m http.server 8000`.

## Data

- The page holds no data. Firebase (Firestore) keeps the data, behind a Google sign-in.
- `firestore.rules` allows only my verified Google account. Paste the rules in the Firebase console after each change.
- The values in `firebase-config.js` are public by design. The security rules protect the data.
- Statement PDFs are stored in Firestore, split into chunks (`files` collection).
