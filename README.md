# Jabble web pages

Static pages App Store Connect needs before release. No build step: plain HTML + one CSS file.

| Page | File | Where it goes in App Store Connect |
|---|---|---|
| Home / marketing | `index.html` | App Information → Marketing URL (optional) |
| Support | `support.html` | Version page → Support URL (**required**) |
| Privacy policy | `privacy.html` | App Privacy → Privacy Policy URL (**required**) |

## Before publishing

Replace the placeholders in all three pages:

- `[DEVELOPER NAME]` – your name or company, as on your developer account
- `[CONTACT EMAIL]` – a support address you check
- `[APP STORE LINK]` – in `index.html`, once the app is live (until then, remove the button)

## Hosting (free options)

- **GitHub Pages:** push this folder to a repo, Settings → Pages → deploy from the main branch. URLs look like `https://<you>.github.io/jabble-pages/privacy.html`.
- **Netlify / Cloudflare Pages:** drag the folder onto their dashboard.

Any HTTPS URL works; Apple just needs the pages to load.

## App Privacy answers ("nutrition label")

The privacy policy matches answering **"No, we do not collect data from this app"**: no analytics, ads or servers. Settings and best scores stay on the device, multiplayer is peer-to-peer, and Game Center data is handled by Apple.

If you later add analytics, crash reporting, ads or a server, update both the label and `privacy.html`.
