# ExpenseIQ — Smart Expense Tracker

## Use it right now (offline, single device)
Just open `index.html` in Chrome, Firefox, or Safari — no internet needed.
Name/PIN setup and the PIN lock work immediately. Fingerprint/Face unlock
and "Add to Home Screen" installation need the app to be hosted online (see
below) because browsers only allow those features over HTTPS.

## Make it a real installable app (Android, iPhone, Desktop) — free, ~10 min
1. Create a free account at https://app.netlify.com (or https://vercel.com,
   or use GitHub Pages).
2. Drag this whole `khaata-app` folder onto Netlify's "Deploy manually" box.
3. Netlify gives you a link like `expenseiq-rafay.netlify.app`.
4. Open that link on your phone:
   - **Android (Chrome):** menu → "Add to Home screen" / "Install app"
   - **iPhone (Safari):** Share button → "Add to Home Screen"
   - **Desktop (Chrome/Edge):** address bar → install icon
5. Now it opens full-screen like a real app, works offline after the first
   load, and fingerprint/Face unlock will work if the device supports it.

## What's new in this version
- Renamed to **ExpenseIQ**, with a new icon
- **Spending insight banner** — compares your current period to the
  previous one and flags the biggest mover
- **Yearly view** added alongside Daily/Weekly/Monthly
- Fixed the broken setup-screen layout
- "Logged in successfully" toast on unlock
- Proper warning dialog (instead of a plain browser popup) before resetting
  PIN/data

## Notes
- All data (expenses, PIN, name) stays on the device only — nothing is sent
  anywhere. There is no cloud account, so data does not sync between devices.
- Use "Export backup" regularly and save the file somewhere safe — it's the
  only way to recover data if a PIN is forgotten or a device is lost.
