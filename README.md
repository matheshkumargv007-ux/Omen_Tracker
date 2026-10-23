# OMENTRACKER — Neon Edition

Daily routine and habit streak PWA using your supplied hooded blue-energy logo and a black / neon-purple / lavender / cyan theme.

## Features
- Daily habit check-ins with current and best streaks
- Home dashboard with today's completion and weekly activity
- Add, edit, and delete habits
- 30-day activity calendar and consistency statistics
- Large, mobile-friendly typography and touch controls
- Local browser storage; progress stays in the browser profile on each device
- Installable PWA with offline app-shell caching after its first successful load

## Run on your laptop (Chrome)
1. Extract this ZIP.
2. Open the extracted `OmenTracker_Neon_App` folder in VS Code.
3. Choose **Terminal → New Terminal**.
4. Run `py -m http.server 5500`.
5. Open `http://localhost:5500` in Chrome.
6. In Chrome, use the install icon in the address bar if shown, or open **⋮ → Cast, save and share → Install page as app**. Wording can vary by Chrome version.

Keep the terminal open while using the local version. `localhost` works for local PWA testing, but a phone cannot use your laptop's `localhost` address to reach the laptop.

## Install on Android Chrome
An installable app must be served over HTTPS for normal phone installation. Publish the *contents* of this folder to a static HTTPS host, for example GitHub Pages:
1. Create a public repository on GitHub.
2. Upload every file in this folder (not the ZIP itself) to the repository root and commit.
3. Open **Settings → Pages**; choose **Deploy from a branch**, branch `main`, folder `/(root)`, then **Save**.
4. Wait for the published `https://...github.io/.../` address shown by GitHub Pages.
5. Open that HTTPS address in Chrome on Android, open **⋮**, and tap **Install app** or **Add to Home screen**; confirm the prompt.

## Notes
- Habit data is stored in `localStorage`, separately in each browser/device; it is not cloud-synced.
- No account, tracking server, or external library is required.
- If you change files after installation, close/reopen the app or refresh the hosted page. Service-worker updates may take a moment to activate.
