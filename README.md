# TowPro Customer PWA

Premium customer-facing Progressive Web App for tow / roadside companies.

## Files
- `index.html` — Customer home (Call Now + Share Location + Add to Home Screen)
- `manifest.json` — PWA manifest (relative paths)
- `sw.js` — Offline cache + push handling
- `api/send-seasonal-push.js` — OneSignal seasonal broadcast
- `vercel.json` — Cron for seasonal push (Oct 15)
- `icons/` — Put real logo here as icon-192.png and icon-512.png

## Soft-ask notifications
Appears only after ~9 seconds (or after user taps location). Never on page load. User must tap "Yes" before the browser permission prompt.

## Deploy
1. Replace all `[PLACEHOLDERS]` with real business data
2. Add real logo to `icons/icon-192.png` and `icons/icon-512.png`
3. Create free OneSignal account → set ONESIGNAL_APP_ID and ONESIGNAL_API_KEY in Vercel
4. Deploy folder to Vercel / Netlify / GitHub Pages
