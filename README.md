# Millan Store

Simple static homepage for Millan Stores — a community-first marketplace for young creators.

## Preview locally

1. Serve the repository root from a simple static server. Example (Python 3):

   ```bash
   python -m http.server 5173
   ```

2. Open http://localhost:5173 in your browser.

## Deploy options

### GitHub Pages (static)

1. In your repository Settings → Pages, set the source to the `main` branch and the root (`/`) folder.
2. Save and wait a minute for your site to publish at `https://<your-username>.github.io/<repo-name>/`.

### Vercel (recommended for simple and dynamic deployments)

1. Sign in to https://vercel.com and import this GitHub repository.
2. Use the default settings. For a static site, no build command is required (leave build command blank) and the Output Directory should be `/`.
3. Deploy — Vercel will provide a production URL.

### Netlify

1. Sign in to https://app.netlify.com and create a new site from Git.
2. Connect your repository and set the build settings (none required for static HTML). Deploy.

## Notes & next steps

- The HTML links to `/index.css` and `/favicon.svg` at the repository root — keep them there.
- Replace analytics placeholders in `index.html` (e.g. `%VITE_ANALYTICS_ENDPOINT%`) with real values or remove the script until configured.
- If this is a Vite/React project (there is a `/src/main.tsx`), decide whether you want this static `index.html` as the app entry or to move the layout into your React app.

If you want, I can also update the site to use a PNG favicon (favicon.ico) and add automatic preview/deploy GitHub Actions workflow.