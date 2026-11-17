# Mind & Money AI — Android PWA starter

This is an installable, phone-friendly web app. It is free and requires no Play Store account.

## Install it on Android

A PWA must be served over HTTPS (or localhost) for installation/offline support. Easiest free method:

1. Extract this ZIP on a computer.
2. Create a free GitHub account if you do not have one.
3. Create a new public repository, for example `mind-money-ai`.
4. Upload `index.html`, `manifest.webmanifest`, `sw.js`, and `icon.svg` to the repository root.
5. In GitHub, open **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then Save.
7. Wait for GitHub Pages to publish. Your app URL will look like `https://YOUR-USERNAME.github.io/mind-money-ai/`.
8. On your Android phone, open that URL in Chrome.
9. Tap Chrome's three-dot menu → **Add to Home screen** or **Install app** → Install/Add.
10. Open the new Mind & Money icon from your home screen.

GitHub Pages is free for public repositories. The repository is public, so do not put private information, passwords, API keys, or financial records in its source files. Your transaction data and book notes are saved in local browser storage on your phone, not uploaded to GitHub. Back up your data with the Export button.

## Features in this starter
- Daily inspiration quotes
- Income, expense and savings tracking
- Savings goal progress
- Stock ticker watchlist with links to Yahoo Finance research pages
- Book/notes library stored locally
- AI prompt builder and link to ChatGPT
- Offline app shell after first successful load

## Important limitations
- This first Android version does not stream live stock prices inside the app. It opens Yahoo Finance for current quotes and research; prices may be delayed.
- The prompt builder prepares a prompt; it does not itself run a local language model. You can paste prompts into ChatGPT or another AI service. A later version can connect to a local Ollama server on your Linux computer, but that computer must be running and reachable on the same network.
- Data is stored in the browser on this phone. Clearing Chrome site data can erase it. Use Export my data for backups.
- Educational tool only; not financial advice and it cannot trade or access brokerage accounts.

## Keep the app updated
When you upload a new version to GitHub Pages, increment the cache name in `sw.js` (for example `mind-money-v2`) so the phone downloads the updated files.
