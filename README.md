# Chrome Web Store — listing kit

Host the `store-site/` folder on any HTTPS site (GitHub Pages, Netlify, Cloudflare Pages, or a path on [mksoltech.com](https://mksoltech.com/)).

## Required URLs for the Developer Dashboard

| Field | Suggested URL |
| --- | --- |
| Homepage | `https://masadaqmk.github.io/ebay-product-alert/` |
| Privacy policy | `https://masadaqmk.github.io/ebay-product-alert/privacy.html` |
| Support email | `mksoltech@gmail.com` |

## Single purpose (paste into store + privacy alignment)

Monitor eBay listing or saved-search URLs the user chooses, using their existing eBay login in Chrome, detect newly appearing items, store watch rules and matches locally, and show browser notifications. The extension does not upload user data to the developer’s servers.

## Short description (132 chars max)

Paste an eBay URL, watch with your browser session, and get alerts when new products appear.

## Detailed description (draft)

Product Alert Watcher watches the eBay search or category URLs you save and notifies you when new listings appear.

Features:
• Add multiple watches with custom check intervals
• Uses your existing eBay sign-in in Chrome
• Local dashboard with stats, charts, and product listing
• Desktop notifications and stacked in-app alerts with sound
• Pause, edit, reset, or delete watches anytime

Privacy:
• Watches and matches stay in chrome.storage on your device
• No MKSOL TECH backend for this extension
• We do not sell your data

Designed & developed by MKSOL TECH (https://mksoltech.com/).
Not affiliated with eBay Inc. Use your own eBay account and follow eBay’s terms.

## Permission justifications (dashboard)

- **storage**: Save watches, matches, and settings locally.
- **cookies**: Read eBay session cookies so fetches use your signed-in browser session.
- **alarms**: Schedule background polling.
- **notifications**: Alert when new products are found.
- **tabs**: Open item pages from notifications/links and reopen the extension app tab.
- **Host permissions (eBay domains)**: Fetch only the eBay URLs the user configures to watch.

## Privacy practices checklist

- [x] Handles user data: Yes (eBay cookies / page content / local watches)
- [x] Used for app functionality only
- [x] Not sold
- [x] Not used for ads / unrelated analytics
- [x] Not transferred to developer servers
- [x] Transferred to eBay only as part of normal HTTPS fetches the user initiates via watches

## Package for upload

1. Zip the extension root **without** `store-site/`, `.git/`, or `scripts/`.
2. Include `manifest.json`, `app/`, `background/`, `lib/`, `icons/`.
3. Capture screenshots of Dashboard, Watches, Product listing, and a toast alert (1280×800 or 640×400).

## Local preview

Open `store-site/index.html` and `store-site/privacy.html` in a browser, or serve the folder:

```bash
npx --yes serve store-site
```
