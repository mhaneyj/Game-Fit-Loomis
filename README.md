# Game-Fit Loomis website

Static site, no build step. Deploys to Vercel as-is.

## Files
- `index.html` — the whole site
- `logo.webp`, `logo.png` — transparent logo
- `og.jpg` — link preview image (texts, iMessage, Facebook)
- `favicon-32.png`, `apple-touch-icon.png`, `icon-512.png` — icons
- `vercel.json` — clean URLs and image caching

## Connect the sign-up form
1. In Google Forms: Send → link icon → copy the link. Use the full `docs.google.com/forms/...` link (uncheck "Shorten URL") so the form embeds inline.
2. Open `index.html`, search for `GOOGLE_FORM_URL`, and paste the link between the quotes.
3. Commit. Vercel redeploys in about 30 seconds.

Until the link is set, the sign-up section shows "Online sign-up opens soon" with the phone number.

## Deploy (first time)
1. Create a GitHub repo (e.g. `gamefit-loomis-site`) and upload these files to it.
2. In Vercel: Add New → Project → import the repo. Framework preset: Other. No build command. Deploy.
3. Custom domain: Vercel project → Settings → Domains → add your domain and follow the DNS records it shows.
