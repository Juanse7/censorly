# Censorly — marketing site

A static, 3-page marketing site for the Censorly app:

- `index.html` — homepage describing the app's features
- `privacy.html` — Privacy Policy (for App Store Connect's "Privacy Policy URL")
- `support.html` — Support page (for App Store Connect's "Support URL")
- `assets/style.css` — shared stylesheet

No build step, no dependencies, no JavaScript framework — just plain HTML/CSS, so it works directly on GitHub Pages.

## Deploy to GitHub Pages

1. Create a new GitHub repository (e.g. `censorly-site`).
2. Upload all the files in this folder to the repository, keeping the `assets` folder structure intact.
3. In the repo, go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**, pick the `main` branch and `/ (root)` folder, then click **Save**.
5. Wait a minute or two — GitHub will give you a URL like:
   `https://<your-username>.github.io/censorly-site/`

## URLs for App Store Connect

Once deployed, use:

- **Privacy Policy URL** → `https://<your-username>.github.io/censorly-site/privacy.html`
- **Support URL** → `https://<your-username>.github.io/censorly-site/support.html`

## Before you publish

A few placeholders to swap out with your real details:

- Email addresses in `privacy.html` and `support.html` (currently `privacy@censorly-app.com`, `support@censorly-app.com`, `feedback@censorly-app.com`)
- The "Download for iPhone / iPad" button links in `index.html` (currently `#`) — point these to your real App Store listing once it's live
- The copyright line in the footer if your legal entity name differs from what you used in App Store Connect's Copyright field

## Notes

- This site only **describes** Censorly's features — it doesn't implement any actual redaction functionality.
- The Privacy Policy content is written to reflect an app that processes everything on-device with no servers. If Censorly's actual implementation uses any analytics, crash reporting, or other third-party SDKs, update the "Third parties" section in `privacy.html` to match reality before publishing — App Store review checks this against your app's actual behavior.
