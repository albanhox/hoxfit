# HoxFit

A personal calorie, macro and weight tracker. One HTML file, no build step, no server.

- **Find the exact product**: search Open Food Facts (millions of labeled products with photos) or scan the barcode with your phone camera.
- **Approve once, one tap forever**: save a product to My Foods and it appears instantly next time.
- **A plan built from your numbers**: BMR and maintenance from the Mifflin-St Jeor formula, a deficit for the pace you pick, macro targets.
- **Weight trend**: daily weigh-ins, 7-day average, goal line, pace, projected goal date.
- **Optional AI assist**: with your own Anthropic API key, type a whole meal or photograph a nutrition label and have it read into numbers.

## Run it

Open `index.html` from any static host. GitHub Pages works out of the box:

1. In this repo go to **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to *Deploy from a branch*, pick **main** and **/ (root)**, then **Save**.
3. A minute later the site is live at `https://<your-user>.github.io/hoxfit/`.
4. On your phone, open that link and use **Add to Home Screen** so it behaves like an app.

The camera (for barcode scanning) requires HTTPS, which GitHub Pages provides.

## Where your data lives

Everything is stored in the browser on the device you use. Nothing is sent anywhere except:

- product searches and barcode lookups to Open Food Facts,
- AI assist requests to the Anthropic API, only if you add your own key.

Use **Plan → Your data → Export backup** now and then, and **Import backup** to move your history to a new phone or browser.

## Files

- `index.html` – the whole app
- `manifest.webmanifest`, `icon.svg`, `icon-180.png`, `icon-512.png` – home-screen install
