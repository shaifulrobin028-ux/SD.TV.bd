# Customization TV

A responsive web app for the provided M3U playlist. It includes channel search, category filters, channel logos, and an HLS player.

## Files
- `index.html` — app interface and player
- `channels.json` — all 34 stream entries parsed from the supplied playlist

## Publish free with GitHub Pages
1. Sign in to GitHub and create a **public** repository named `customization-tv`.
2. Upload `index.html` and `channels.json` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**, choose `main` and `/(root)`, then save.
5. Wait for GitHub Pages to publish. Your address will look like `https://YOUR-USERNAME.github.io/customization-tv/`.

## Use your own domain
If you own a domain such as `customizationtv.com`, add it in **Settings → Pages → Custom domain** and follow GitHub's DNS instructions at your domain registrar. You must own/control the domain; this project does not register it for you.

## Important playback notes
- This is a playlist player, not a stream host or proxy.
- The original playlist contains a mix of HTTP and HTTPS URLs. Browsers may block HTTP streams on an HTTPS GitHub Pages site, and some providers block cross-origin (CORS) browser playback. A channel may therefore fail even if it works in a dedicated IPTV app.
- Playback success depends on the stream provider and your permission to access it.
- The original playlist included a VLC user-agent option for one stream. Browser JavaScript cannot reliably set a custom User-Agent header, so that particular stream may not play in a web browser.
- Check stream authorization and rights before publishing or sharing this site.
