# Cash Flow (web app)

Same app as the iOS version, as a web page you add to your home screen. No Mac, no Xcode, no App Store. Data is stored only in your phone's browser.

## Put it online (free, about 5 minutes)

The page needs to be served from an https address so the phone can install it. Pick one:

**Netlify Drop (easiest, no account needed for a trial)**
1. Unzip this folder.
2. Go to https://app.netlify.com/drop and drag the whole folder onto the page.
3. It gives you an address like `https://something.netlify.app`. Sign up (free) if you want to keep it permanently.

**GitHub Pages** (if you have a GitHub account)
1. Create a new public repository and upload all the files in this folder.
2. Settings > Pages > deploy from the main branch.
3. Your address is `https://<you>.github.io/<repo>/`.

The address is public, but your data is not on it. Entries never leave your phone.

## Install on the iPhone

1. Open the address in **Safari** (it must be Safari, not Chrome).
2. Tap Share > **Add to Home Screen** > Add.
3. Open it from the home-screen icon. Enter your data there, not in the Safari tab: they store data separately.

## Install on Android

Open the address in Chrome, menu > **Install app** (or Add to Home screen).

## Your data

- Stored in the browser on that phone only. Removing the app icon or clearing site data erases it.
- Settings > Export has a CSV for spreadsheets and a JSON backup you can restore from.
- To move to a new phone: Export the JSON backup, then Restore it there.
- If you edit `index.html` later, change the version in `sw.js` (`cashflow-v1` to `cashflow-v2`) so phones pick up the update.
